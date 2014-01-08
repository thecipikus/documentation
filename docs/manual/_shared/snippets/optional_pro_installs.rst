Optional TubePress Pro Installations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Due to licensing restrictions, TubePress Pro does not ship with every library that the free WordPress plugin includes.
However it's very easy to install these optional libraries manually. This section provides installation instructions.

JW Player (version 5.x)
~~~~~~~~~~~~~~~~~~~~~~~

TubePress can use `JW Player <http://www.jwplayer.com/>`_ 5.10 to play YouTube videos. We are working to
integrate JW Player 6.x, but this feature is not yet ready for production.

 1. Download the file ``player.swf``
    from `here <http://developer.longtailvideo.com/trac/browser/tags/mediaplayer-5.10/player.swf>`_.
 2. Upload the file to your TubePress Pro installation at
    ``<tubepress_home>/src/main/web/flash/longtail/player.swf``.

Shadowbox.js
~~~~~~~~~~~~

 1. Download Shadowbox.js from `here <http://www.shadowbox-js.com/download.html>`_.
    The image below shows the required options when configuring your download.
    **You may select additional checkboxes (though not recommended), but make sure that at least the settings
    shown are chosen.**

    .. image:: ../_shared/images/shadowbox_download.png

 2. The download will save to a file named something like ``shadowbox-3.0.3.zip``. Unzip this file, and it will
    expand into a directory named ``shadowbox-3.0.3``.

 3. Copy the *contents* of this directory (not the directory itself) to your TubePress Pro installation at
    ``<tubepress_home>/src/main/web/players/shadowbox/lib/``.

 4. *Optional*. You may see scrollbars in the Shadowbox.js display. To fix this, simply edit ``lib/shadowbox.css``.
    On line 8, remove the ``overflow:auto`` attribute. i.e. change it from ::

      #sb-player.html{height:100%;overflow:auto;}
    to ::

      #sb-player.html{height:100%;}