Vimeo All Access Options
========================

This page documents the options available with the :doc:`../../../manual/add-ons/vimeo-all-access/index` add-on
for TubePress.

.. _option-vimeoApiAccessToken:

.. index::
   single: options (by name); vimeoApiAccessToken
   single: video feed; private Vimeo videos

``vimeoApiAccessToken``
#######################

+------------------------+------------------------------------------------------------------------------------------+
| **Option name**        | ``vimeoApiAccessToken``                                                                  |
+------------------------+------------------------------------------------------------------------------------------+
| Description            | The API secret that TubePress will use when communicating with Vimeo.                    |
+------------------------+------------------------------------------------------------------------------------------+
| Provided with          | * All cloud-based TubePress distributions                                                |
|                        | * :doc:`Vimeo All Access add-on <../../../manual/add-ons/vimeo-all-access/index>` add-on |
+------------------------+------------------------------------------------------------------------------------------+
| Default value          | *empty*                                                                                  |
+------------------------+------------------------------------------------------------------------------------------+
| Valid values           | Any valid Vimeo API access token                                                         |
+------------------------+------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress vimeoApiAccessToken="..."]``                                                |
+------------------------+------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('vimeoApiAccessToken="..."');``                      |
+------------------------+------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apps/new>`_                                      |
+------------------------+------------------------------------------------------------------------------------------+

.. _option-vimeoApiAccessTokenSecret:

.. index::
   single: options (by name); vimeoApiAccessTokenSecret
   single: video feed; private Vimeo videos

``vimeoApiAccessTokenSecret``
#############################

+------------------------+-----------------------------------------------------------------------------------+
| **Option name**        | ``vimeoApiAccessTokenSecret``                                                     |
+------------------------+-----------------------------------------------------------------------------------+
| Description            | The API secret that TubePress will use when communicating with Vimeo.             |
+------------------------+-----------------------------------------------------------------------------------+
| Provided with          | * All cloud-based TubePress distributions                                         |
|                        | * :doc:`Vimeo All Access add-on <../../../manual/add-ons/vimeo-all-access/index>` |
+------------------------+-----------------------------------------------------------------------------------+
| Default value          | *empty*                                                                           |
+------------------------+-----------------------------------------------------------------------------------+
| Valid values           | Any valid Vimeo API access token secret                                           |
+------------------------+-----------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress vimeoApiAccessTokenSecret="..."]``                                   |
+------------------------+-----------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('vimeoApiAccessTokenSecret="..."');``         |
+------------------------+-----------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apps/new>`_                               |
+------------------------+-----------------------------------------------------------------------------------+

.. |br| raw:: html

  <br />
