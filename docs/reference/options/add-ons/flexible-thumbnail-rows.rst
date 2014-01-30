Flexible Thumbnail Row Options
==============================

This page documents the options available with the :doc:`../../../manual/add-ons/flexible-thumbnail-rows/index`
add-on for TubePress.

.. _option-flexibleThumbnailRows:

.. index::
   single: options (by name); flexibleThumbnailRows
   single: thumbnails; flexible row height

``flexibleThumbnailRows``
#########################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``flexibleThumbnailRows``                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Automatically adjust the height of thumbnail rows in TubePress |br|                        |
|                        | galleries, ensuring that the metadata (runtime, title, description, |br|                   |
|                        | etc) for each video is completely visible                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | :doc:`../../../manual/add-ons/flexible-thumbnail-rows/index` add-on                        |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                                                          |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress flexibleThumbnailRows="true"]``                                               |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('flexibleThumbnailRows="true"');``                     |
+------------------------+--------------------------------------------------------------------------------------------+

.. |br| raw:: html

  <br />
