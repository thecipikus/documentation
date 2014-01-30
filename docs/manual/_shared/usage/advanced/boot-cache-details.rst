.. note:: The rest of this section details the contents of ``config/boot.json`` for advanced users. Most users can skip this section.

Let's examine each piece of the file...

.. code-block:: javascript

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
       }
   }

This section of the file enables or disables the caching of individual elements of TubePress's internals.
Most users will set all of these elements to either ``true`` or ``false``.

.. code-block:: javascript

   "killer-key" : "tubepress_boot_cache_kill",

The killer key" can be used to remotely and securely clear the boot cache. The value of ``killer-key`` can be used
as a query parameter to signal to TubePress to clear the boot cache. e.g. if the value of ``killer-key`` is
``456xyz``, then ``456xyz=true`` to the URL of a page using TubePress will clear the entire boot cache.

.. code-block:: javascript

   "dir" : null

The ``dir`` option allows you to manually configure a directory where TubePress will store its boot cache.
If you leave its value as null, TubePress will attempt to use the system's cache directory.

.. code-block:: javascript

   "add-ons" : {

       "blacklist": []
   },

This section allows you to identify, by name, a set of add-ons that will be excluded from TubePress. If you are not
using a particular add-on, adding it to the blacklist will improve TubePress's performance.

.. code-block:: javascript

   "classloader" : {

       "enabled" : true
   }

By default, TubePress uses its own high-performance `PSR-0 <https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md>`_ compliant
class loader. If you would like to use a class loader defined elsewhere, you can set this value to ``false``.