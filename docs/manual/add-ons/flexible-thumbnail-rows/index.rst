Flexible Thumbnail Rows
=======================

.. contents:: On This Page
   :local:

.. _flexrows-intro:

Introduction
--------------

This add-on automatically adjusts the height of thumbnail rows in TubePress galleries, ensuring that the metadata
(runtime, title, description, etc) for each video is completely visible. Without this add-on, TubePress uses a fixed
height for the thumbnail rows, and any metadata that is taller than the row will be cut off.

.. image:: images/overview.png

.. _flexrows-manuals:

Manuals
---------

.. _flexrows-manual-wordpress:

TubePress for WordPress
^^^^^^^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/53-flexible-thumbnail-rows/>`_.
 2. Unzip the file you downloaded (``flexible-thumbnail-rows_x_y_z.zip``) into the ``add-ons`` subdirectory of your
    :ref:`TubePress Content Directory <wordpress-tubepress-content-directory>`.
 3. Configure this add-on from ``WP Admin > Settings > TubePress``. Navigate to the "Thumbnails" tab
    and scroll to the bottom of the page. There you will see a checkbox which enables/disables the add-on.

    .. image:: images/use-in-wp.png

.. _flexrows-usage-manual-php-wptemplates:

Standalone PHP
^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/53-flexible-thumbnail-rows/>`_.
 2. Unzip the file you downloaded (``flexible-thumbnail-rows_x_y_z.zip``) into the ``add-ons`` subdirectory of your
    :ref:`TubePress Content Directory <standalone-tubepress-content-directory>`.
 3. This add-on introduces the :ref:`flexibleThumbnailRows <option-flexibleThumbnailRows>` option that you may supply to ``TubePressPro::getHtmlForShortcode()``. e.g.

    .. code-block:: php

       <?php

       print TubePressPro::getHtmlForShortcode('mode="user" userValue="3hough" flexibleThumbnailRows="true"');

.. _flexrows-usage-wix:

TubePress for Wix
^^^^^^^^^^^^^^^^^

This add-on is pre-installed for users of cloud-based TubePress installations
(e.g. TubePress Express, :doc:`TubePress for Wix <../../wix/index>`). Here's how to use it.

 1. Open up the :ref:`full settings page <wix-configuring-full>` for your TubePress instance.
 2. In the window that opens, navigate to the "Thumbnails" tab and scroll down to the "Flexible Thumbnail Rows" box:

   .. image:: images/use-in-wix.png

 3. Enable or disable the add-on with the checkbox.
 4. Click the "Save" button.