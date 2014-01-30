QuickPlay
=========

.. contents:: On This Page
   :local:

.. _vimeo-all-access-intro:

Introduction
--------------

This TubePress add-on replaces video thumbnail images with fully-functional embedded video players. :ref:`Among other things <quickplay-show-latest-vid>`, this allows your users to watch your videos right within the context of your gallery.

.. image:: images/overview.png

.. note:: This add-on is currently only available for the downloadable TubePress distributions

Manuals
----------

.. _quickplay-manual-wordpress:

TubePress for WordPress
^^^^^^^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/49-vimeo-all-access/>`_.
 2. Unzip the file you downloaded (``quickplay_x_y_z.zip``) into the ``add-ons`` subdirectory of your :ref:`TubePress Content Directory <wordpress-tubepress-content-directory>`.
 3. Copy (or symlink) the directory at ``wp-content/tubepress-content/add-ons/quickplay_x.y.z/tubepress-theme`` **to** ``wp-content/tubepress-content/themes/quickplay``
 4. Anytime you :ref:`add TubePress to a post or page <wordpress-posts-pages-usage>`, set the options ``enableQuickplay='true'`` and ``theme='quickplay'``. e.g.

    .. code-block:: php

       [tubepress enableQuickplay="true" theme="quickplay" ... ]

.. _quickplay-manual-php:

TubePress for PHP
^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/49-vimeo-all-access/>`_.
 2. Unzip the file you downloaded (``quickplay_x_y_z.zip``) into the ``add-ons`` subdirectory of your
    :ref:`TubePress Content Directory <standalone-tubepress-content-directory>`.
 3. Copy (or symlink) the directory at ``tubepress-content/add-ons/quickplay_x.y.z/tubepress-theme`` **to** ``tubepress-content/themes/quickplay``
 4. Anytime you :ref:`add TubePress to a page <basic-standalone-configuration>`, set the options ``enableQuickplay='true'`` and ``theme='quickplay'``. e.g.

    .. code-block:: php

       <?php

       print TubePressPro::getHtmlForShortcode('enableQuickplay="true" theme="quickplay" ... ');

.. _quickplay-additional-notes:

Additional Notes
----------------

.. _quickplay-height-width:

Controlling Height and Width
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To control the height and width of the embedded video players, you can simply use the :ref:`embeddedHeight <option-embeddedHeight>`
and :ref:`embeddedWidth <option-embeddedWidth>` options. :ref:`thumbHeight <option-thumbHeight>` and
:ref:`thumbWidth <option-thumbWidth>` are **ignored** when this add-on is in use.

.. _quickplay-show-latest-vid:

Show the Latest Video from a Collection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A common question we get from customers is

    How can I have an embedded video player that automatically shows the latest video from my YouTube or Vimeo channel?

With QuickPlay, this is easy. The trick is to set :ref:`resultCountCap <option-resultCountCap>` to ``1`` and
:ref:`orderBy <option-orderBy>` to ``newest``.

For instance, say that you'd like to show the latest video from YouTube user ``engineerguyvideo``. WordPress users would use
the following shortcode:

.. code-block:: php

   [tubepress mode='user' userValue='engineerguyvideo' resultCountCap='1' orderBy='newest' enableQuickplay='true' theme='quickplay' embeddedWidth='480' embeddedHeight='270']

Similarly, PHP users could use the following invocation of ``TubePressPro::getHtmlForShortcode()``:

.. code-block:: php

   <?php

       TubePressPro::getHtmlForShortcode("mode='user' userValue='engineerguyvideo' resultCountCap='1' orderBy='newest' enableQuickplay='true' theme='quickplay' embeddedWidth='480' embeddedHeight='270'");

The result is an always-updating, fully customizable single video embed that you can embed anywhere on your site.

.. image:: images/latest-vid.png
