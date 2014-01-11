Vimeo Options
======================

.. contents:: On This Page
   :local:

.. _vimeo-gallery-sources:

Gallery Sources
---------------

.. contents:: Gallery Sources
   :local:

.. _mode-vimeoAlbum:

.. index::
   single: mode; vimeoAlbum

``vimeoAlbum``
#################################

+------------------------+--------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoAlbum``                                                                             |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Videos from a Vimeo album. The album is identified by the value |br|                       |
|                        | supplied to the ``vimeoAlbumValue`` option.                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoAlbum" vimeoAlbumValue="852694"]``                                 |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoAlbum" vimeoAlbumValue="852694"');``       |
+------------------------+--------------------------------------------------------------------------------------------+
| Vimeo documentation  | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.albums.getVideos>`_      |
+------------------------+--------------------------------------------------------------------------------------------+

.. _mode-vimeoAppearsIn:

.. index::
   single: mode; vimeoAppearsIn

``vimeoAppearsIn``
#################################

+------------------------+----------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoAppearsIn``                                                                                 |
+------------------------+----------------------------------------------------------------------------------------------------+
| Description            | Vimeo videos in which a given user appears. The Vimeo user is identified |br|                      |
|                        | you supply to the ``vimeoAppearsInValue`` attribute.                                               |
+------------------------+----------------------------------------------------------------------------------------------------+
| Notes                  | Limited to 50 videos.                                                                              |
+------------------------+----------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoAppearsIn" vimeoAppearsInValue="dabrainkilla"]``                           |
+------------------------+----------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoAppearsIn" vimeoAppearsInValue="dabrainkilla"');`` |
+------------------------+----------------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getAppearsIn>`_         |
+------------------------+----------------------------------------------------------------------------------------------------+

.. _mode-vimeoChannel:

.. index::
   single: mode; vimeoChannel

``vimeoChannel``
#################################

+------------------------+--------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoChannel``                                                                           |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Videos from a Vimeo channel. The channel is identified by the value |br|                   |
|                        | supplied to the ``vimeoChannelValue`` option.                                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoChannel" vimeoChannelValue="besthd"]``                             |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoChannel" vimeoChannelValue="besthd"');``   |
+------------------------+--------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.channels.getVideos>`_  |
+------------------------+--------------------------------------------------------------------------------------------+

.. _mode-vimeoCreditedTo:

.. index::
   single: mode; vimeoCreditedTo

``vimeoCreditedTo``
#################################

+------------------------+--------------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoCreditedTo``                                                                                    |
+------------------------+--------------------------------------------------------------------------------------------------------+
| Description            | Vimeo videos for which a particular user has either uploaded or appeared in. |br|                      |
|                        | The Vimeo user is identified by the value supplied to the vimeoCreditedToValue option.                 |
+------------------------+--------------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoCreditedTo" vimeoCreditedToValue="thunderingherd"]``                           |
+------------------------+--------------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoCreditedTo" vimeoCreditedToValue="thunderingherd"');`` |
+------------------------+--------------------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getAll>`_                   |
+------------------------+--------------------------------------------------------------------------------------------------------+

.. _mode-vimeoGroup:

.. index::
   single: mode; vimeoGroup

``vimeoGroup``
#################################

+------------------------+----------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoGroup``                                                                               |
+------------------------+----------------------------------------------------------------------------------------------+
| Description            | Videos from a Vimeo group. The group is identified by the value |br|                         |
|                        | supplied to the ``vimeoGroupValue`` option.                                                  |
+------------------------+----------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoGroup" vimeoGroupValue="underachievers"]``                           |
+------------------------+----------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoGroup" vimeoGroupValue="underachievers"');`` |
+------------------------+----------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.channels.getVideos>`_    |
+------------------------+----------------------------------------------------------------------------------------------+

.. _mode-vimeoLikes:

.. index::
   single: mode; vimeoLikes

``vimeoLikes``
#################################

+------------------------+------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoLikes``                                                                           |
+------------------------+------------------------------------------------------------------------------------------+
| Description            | Vimeo videos that a particular user has "liked." The Vimeo user |br|                     |
|                        | is identified by the value supplied to the ``vimeoLikesValue`` option.                   |
+------------------------+------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoLikes" vimeoLikesValue="besthd"]``                               |
+------------------------+------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoLikes" vimeoLikesValue="besthd"');``     |
+------------------------+------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.groups.getVideos>`_  |
+------------------------+------------------------------------------------------------------------------------------+

.. _mode-vimeoSearch:

.. index::
   single: mode; vimeoSearch

``vimeoSearch``
#################################

+------------------------+---------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoSearch``                                                                                   |
+------------------------+---------------------------------------------------------------------------------------------------+
| Description            | Vimeo videos that match a supplied search term. The search term |br|                              |
|                        | is identified by the value supplied to the ``vimeoSearchValue option``.                           |
+------------------------+---------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoSearch" vimeoSearchValue="rainbow alligator"]``                           |
+------------------------+---------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoSearch" vimeoSearchValue="rainbow alligator"');`` |
+------------------------+---------------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.videos.search>`_              |
+------------------------+---------------------------------------------------------------------------------------------------+

.. _mode-vimeoUploadedBy:

.. index::
   single: mode; vimeoUploadedBy

``vimeoLikes``
#################################

+------------------------+------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``vimeoUploadedBy``                                                                            |
+------------------------+------------------------------------------------------------------------------------------------+
| Description            | Vimeo videos uploaded by a particular user. The Vimeo user is |br|                             |
|                        | identified by the value supplied to the ``vimeoUploadedByValue`` option.                       |
+------------------------+------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="vimeoUploadedBy" vimeoUploadedByValue="ehough"]``                           |
+------------------------+------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="vimeoUploadedBy" vimeoUploadedByValue="ehough"');`` |
+------------------------+------------------------------------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getUploaded>`_      |
+------------------------+------------------------------------------------------------------------------------------------+

Embedded Video Player
-----------------------

.. contents:: Embedded Video Player
   :local:

.. _option-playerColor:

.. index::
   single: playerColor

``playerColor``
#################################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``playerColor``                                                                            |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | The highlight color of the Vimeo video player.                                             |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``000000``                                                                                 |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | Any six hexadecimal characters representing an `HTML color`_.                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress playerColor="A32638"]``                                                       |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('playerColor="A32638"');``                             |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <http://developer.vimeo.com/player/embedding#universal-parameters>`_           |
+------------------------+--------------------------------------------------------------------------------------------+

.. _HTML color: http://en.wikipedia.org/wiki/Web_colors#Hex_triplet

.. _vimeo-video-feed:

Video Feed
--------------

.. contents:: Video Feed Options
   :local:

.. _option-vimeoKey:

.. index::
   single: vimeoKey

``vimeoKey``
#################################

+------------------------+--------------------------------------------------------------------+
| **Option name**        | ``vimeoKey``                                                       |
+------------------------+--------------------------------------------------------------------+
| Description            | The API key that TubePress will use when communicating with Vimeo. |
+------------------------+--------------------------------------------------------------------+
| Provided with          | All downloadable TubePress distributions                           |
+------------------------+--------------------------------------------------------------------+
| Default value          | *empty*                                                            |
+------------------------+--------------------------------------------------------------------+
| Valid values           | Any valid Vimeo API key                                            |
+------------------------+--------------------------------------------------------------------+
| Shortcode example      | ``[tubepress vimeoKey="..."]``                                     |
+------------------------+--------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('vimeoKey="..."');``           |
+------------------------+--------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apps/new>`_                |
+------------------------+--------------------------------------------------------------------+

.. _option-vimeoSecret:

.. index::
   single: vimeoSecret

``vimeoSecret``
#################################

+------------------------+-----------------------------------------------------------------------+
| **Option name**        | ``vimeoSecret``                                                       |
+------------------------+-----------------------------------------------------------------------+
| Description            | The API secret that TubePress will use when communicating with Vimeo. |
+------------------------+-----------------------------------------------------------------------+
| Provided with          | All downloadable TubePress distributions                              |
+------------------------+-----------------------------------------------------------------------+
| Default value          | *empty*                                                               |
+------------------------+-----------------------------------------------------------------------+
| Valid values           | Any valid Vimeo API secret                                            |
+------------------------+-----------------------------------------------------------------------+
| Shortcode example      | ``[tubepress vimeoSecret="..."]``                                     |
+------------------------+-----------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('vimeoSecret="..."');``           |
+------------------------+-----------------------------------------------------------------------+
| Vimeo documentation    | `Click here <http://developer.vimeo.com/apps/new>`_                   |
+------------------------+-----------------------------------------------------------------------+


.. _vimeo-meta-display:

Video Meta Display
---------------------

.. _option-likes:

.. index::
   single: likes

``likes``
#################################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``likes``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Toggle display of the number of times the video has been "liked".                          |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress likes="true"]``                                                               |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('likes="true"');``                                     |
+------------------------+--------------------------------------------------------------------------------------------+

.. |br| raw:: html

  <br />
