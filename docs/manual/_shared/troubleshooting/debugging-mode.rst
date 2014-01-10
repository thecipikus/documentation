TubePress's debug mode will print a huge amount of logging statements to the screen. It will describe in (extreme)
detail what TubePress is doing behind the scenes.

.. image:: ../_shared/troubleshooting/images/debugging_mode.png

To use it, you just need to add ``tubepress_debug=true`` to the URL string (in your browser's address bar) of any
page that uses TubePress on it. For instance, if the TubePress page you're trying to debug has an address of

  ``http://ehough.com/?page_id=19``

then you should add ``tubepress_debug=true`` to the URL to enable debugging:

 ``http://ehough.com/?page_id=19&tubepress_debug=true``

Most of the debug output is self-explanatory. If the output is cut off unexpectedly, it's likely that TubePress
encountered a fatal error. Check your PHP error logs for more information.