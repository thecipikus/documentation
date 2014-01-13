Enabling the cache is easy; you'll just need a text editor. Here's how to do it...

 1. Ensure that TubePress debugging is enabled.

    In standalone PHP environments, this is enabled by default. In WordPress environments, ensure the box at WP Admin > Settings > TubePress > Advanced > Enable Debugging is ticked. This will allow you to verify that the cache is working.

 2. TubePress's boot process is controlled by a single file located within your TubePress content directory at
    ``config/boot.json``. In TubePress 3.1.0+, this file and the config directory are included by default. In older
    versions of TubePress, simply create ``tubepress-content/config/boot.json`` and fill it with the following contents:

    .. code-block:: javascript

       {
           "cache" : {
               "ioc-container" : {
                   "enabled" : false
               },
               "add-ons" : {
                   "enabled" : false
               },
               "classloader" : {
                   "enabled" : false
               },
               "option-descriptors" : {
                   "enabled" : false
               },
               "killer-key" : "tubepress_boot_cache_kill",
               "dir" : null
           },
           "add-ons" : {
               "blacklist": []
           },
           "classloader" : {
               "enabled" : true
           }
        }

 3. Replace each instance of ``false`` with ``true``, and set the value of ``killer-key`` to a random string.
    Your copy of ``tubepress-content/config/boot.json`` should now look something like this:

    .. code-block:: javascript

       {
           "cache" : {
               "ioc-container" : {
                   "enabled" : true
               },
               "add-ons" : {
                   "enabled" : true
               },
               "classloader" : {
                   "enabled" : true
               },
               "option-descriptors" : {
                   "enabled" : true
               },
               "killer-key" : "tIEKrw84k7z760811D815363425xa15370W",
               "dir" : null
           },
           "add-ons" : {
               "blacklist": []
           },
           "classloader" : {
               "enabled" : true
           }
        }

 4. Verify that the boot cache is working by examining your TubePress debug output. You should see something similar
    to the following:

    .. code-block:: text
       :emphasize-lines: 2,3,4,6,7,9,11,12

           Default Boot Config Service: Attempting to read boot config from /var/www/ttg.lan/wordpress/wp-content/tubepress-content/config/boot.json
           Default Boot Config Service: Successfully read boot config from /var/www/ttg.lan/wordpress/wp-content/tubepress-content/config/boot.json
           Default Boot Config Service: classloader caching is enabled
           Default Boot Config Service: add-ons caching is enabled
           ...
           Default Add-on Discoverer: Successfully hydrated from cache file at ... /serialized-addons.txt
           Default Boot Config Service: ioc-container caching is enabled
           ...
           Default IOC Boot Helper: Successfully hydrated from cache file at ... /cached-ioc-container.php
           ...
           Default Boot Config Service: option-descriptors caching is enabled
           Default Option Descriptor Reference: Successfully hydrated from cache file at ... /serialized-option-descriptors.txt
           ...
           TubePress Bootstrapper: Boot completed in 28.892893 milliseconds
        ..

           If your debug output is missing any of the highlighted phrases, it means that something is misconfigured.
           Feel free to post a question in `the forum <https://community.tubepress.com/>`_ to get help.