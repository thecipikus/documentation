After adding or removing TubePress add-ons, you'll need to clear the boot cache so TubePress can recognize
the changes to your installation.

You can clear the cache using any web browser, and you'll simply need to know the value of ``killer-key`` that was set
in your ``config/boot.json``. As an example, suppose that the value of ``killer-key`` is ``abc123``, then you would
add ``abc123=true`` to the end of any URL where TubePress is used to clear the cache. For instance,

.. code-block:: php

   http://myblog.com/videos?abc123=true