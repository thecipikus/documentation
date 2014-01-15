YouTube Black Bars Remover
==========================

.. contents:: On This Page
   :local:

.. _youtube-bbr-intro:

Introduction
--------------

Most YouTube video thumbnails have horizontal black bars on the top and bottom. This TubePress add-on completely
removes these bars, leaving behind a clean and more professional image.

.. note:: Use of this add-on will change the aspect ratio of YouTube thumbnails from 4:3 to 16:9. You will likely want to adjust your settings for :ref:`thumbHeight <option-thumbHeight>` and :ref:`thumbWidth <option-thumbWidth>`.

.. image:: images/overview.jpg

.. _youtube-bbr-manuals:

Manuals
---------

.. _youtube-bbr-manual-wordpress:

TubePress for WordPress
^^^^^^^^^^^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/42-youtube-black-bars-remover/>`_.
 2. Unzip the file you downloaded (``youtube-black-bars-remover_x_y_z.zip``) into the ``add-ons`` subdirectory of your
    :ref:`TubePress Content Directory <wordpress-tubepress-content-directory>`.
 3. Configure this add-on from ``WP Admin > Settings > TubePress``. Navigate to the "Thumbnails" tab
    and scroll to the bottom of the page. There you will see a checkbox which enables/disables the black bar removal.

    .. image:: images/use-in-wp.png

.. _youtube-bbr-usage-manual-php-wptemplates:

Standalone PHP
^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/42-youtube-black-bars-remover/>`_.
 2. Unzip the file you downloaded (``youtube-black-bars-remover_x_y_z.zip``) into the ``add-ons`` subdirectory of your
    :ref:`TubePress Content Directory <standalone-tubepress-content-directory>`.
 3. This add-on introduces the :ref:`youtubeHideBlackBars <option-youtubeHideBlackBars>` option that you may supply to ``TubePressPro::getHtmlForShortcode()``. e.g.

    .. code-block:: php

       <?php

       print TubePressPro::getHtmlForShortcode('mode="user" userValue="3hough" youtubeHideBlackBars="true"');
