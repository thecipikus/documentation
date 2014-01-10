TubePress Options
=================

.. contents:: On This Page
   :local:

Embedded Video Player
---------------------

.. _option-autonext:

.. index::
   single: autoNext

``autoNext``
############

+------------------------+-----------------------------------------------------------+
| **Option name**        | ``autoNext``                                              |
+------------------------+-----------------------------------------------------------+
| Description            | Automatically start the next video in a gallery when |br| |
|                        | playback of a video finishes.                             |
+------------------------+-----------------------------------------------------------+
| Provided with          | * TubePress Pro                                           |
|                        | * Any cloud-hosted TubePress                              |
+------------------------+-----------------------------------------------------------+
| Default value          | ``false``                                                 |
+------------------------+-----------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                     |
+------------------------+-----------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                         |
+------------------------+-----------------------------------------------------------+
| Shortcode example      | ``[tubepress autoNext="true"]``                           |
+------------------------+-----------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('autoNext="true"');`` |
+------------------------+-----------------------------------------------------------+

.. _option-autoplay:

.. index::
   single: autoplay

``autoplay``
############

+------------------------+-----------------------------------------------------------+
| **Option name**        | ``autoplay``                                              |
+------------------------+-----------------------------------------------------------+
| Description            | Automatically start video playback of *any* embedded |br| |
|                        | video when the page is loaded.                            |
+------------------------+-----------------------------------------------------------+
| Provided with          | * All TubePress distributions                             |
+------------------------+-----------------------------------------------------------+
| Default value          | ``false``                                                 |
+------------------------+-----------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                     |
+------------------------+-----------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                         |
+------------------------+-----------------------------------------------------------+
| Shortcode example      | ``[tubepress autoplay="true"]``                           |
+------------------------+-----------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('autoplay="true"');`` |
+------------------------+-----------------------------------------------------------+

.. _option-embeddedHeight:

.. index::
   single: embeddedHeight

``embeddedHeight``
##################

+------------------------+----------------------------------------------------------------+
| **Option name**        | ``embeddedHeight``                                             |
+------------------------+----------------------------------------------------------------+
| Description            | The height, in pixels, of the embedded video player |br|       |
|                        | that TubePress builds.                                         |
+------------------------+----------------------------------------------------------------+
| Provided with          | * All TubePress distributions                                  |
+------------------------+----------------------------------------------------------------+
| Default value          | ``350``                                                        |
+------------------------+----------------------------------------------------------------+
| Valid values           | Any positive integer                                           |
+------------------------+----------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                              |
+------------------------+----------------------------------------------------------------+
| Shortcode example      | ``[tubepress embeddedHeight="350"]``                           |
+------------------------+----------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('embeddedHeight="350"');`` |
+------------------------+----------------------------------------------------------------+

.. _option-embeddedWidth:

.. index::
   single: embeddedWidth

``embeddedWidth``
#################

+------------------------+----------------------------------------------------------------+
| **Option name**        | ``embeddedWidth``                                              |
+------------------------+----------------------------------------------------------------+
| Description            | The width, in pixels, of the embedded video player |br|        |
|                        | that TubePress builds.                                         |
+------------------------+----------------------------------------------------------------+
| Provided with          | * All TubePress distributions                                  |
+------------------------+----------------------------------------------------------------+
| Default value          | ``425``                                                        |
+------------------------+----------------------------------------------------------------+
| Valid values           | Any positive integer                                           |
+------------------------+----------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                              |
+------------------------+----------------------------------------------------------------+
| Shortcode example      | ``[tubepress embeddedWidth="350"]``                            |
+------------------------+----------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('embeddedWidth="350"');``  |
+------------------------+----------------------------------------------------------------+

.. _option-enablejsapi:

.. index::
   single: enableJsApi

``enableJsApi``
###############

+------------------------+-----------------------------------------------------------------+
| **Option name**        | ``enableJsApi``                                                 |
+------------------------+-----------------------------------------------------------------+
| Description            | Enable or disable the TubePress JavaScript API for this |br|    |
|                        | gallery. Enabling this API incurs a tiny performance |br|       |
|                        | overhead, but is required for some features                     |
|                        | (such as :ref:`autoNext <option-autoNext>`).                    |
+------------------------+-----------------------------------------------------------------+
| Provided with          | * TubePress Pro                                                 |
+------------------------+-----------------------------------------------------------------+
| Default value          | ``true``                                                        |
+------------------------+-----------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                           |
+------------------------+-----------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                               |
+------------------------+-----------------------------------------------------------------+
| Shortcode example      | ``[tubepress enableJsApi="true"]``                              |
+------------------------+-----------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('enableJsApi="true"');``    |
+------------------------+-----------------------------------------------------------------+

.. _option-lazyPlay:

.. index::
   single: lazyPlay

``lazyPlay``
############

+------------------------+-----------------------------------------------------------------+
| **Option name**        | ``lazyPlay``                                                    |
+------------------------+-----------------------------------------------------------------+
| Description            | If enabled, video playback will auto-start after users  |br|    |
|                        | clicks a video's thumbnail.                                     |
+------------------------+-----------------------------------------------------------------+
| Provided with          | * All TubePress distributions                                   |
+------------------------+-----------------------------------------------------------------+
| Default value          | ``true``                                                        |
+------------------------+-----------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                           |
+------------------------+-----------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                               |
+------------------------+-----------------------------------------------------------------+
| Shortcode example      | ``[tubepress lazyPlay="true"]``                                 |
+------------------------+-----------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('lazyPlay="true"');``       |
+------------------------+-----------------------------------------------------------------+

.. _option-loop:

.. index::
   single: loop

``loop``
############

+------------------------+-------------------------------------------------------------------+
| **Option name**        | ``loop``                                                          |
+------------------------+-------------------------------------------------------------------+
| Description            | If enabled, immediately restart playback of each video after |br| |
|                        | it finishes.                                                      |
+------------------------+-------------------------------------------------------------------+
| Provided with          | * All TubePress distributions                                     |
+------------------------+-------------------------------------------------------------------+
| Default value          | ``false``                                                         |
+------------------------+-------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                             |
+------------------------+-------------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                                 |
+------------------------+-------------------------------------------------------------------+
| Shortcode example      | ``[tubepress loop="true"]``                                       |
+------------------------+-------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('loop="true"');``             |
+------------------------+-------------------------------------------------------------------+

.. _option-playerImplementation:

.. index::
   single: playerImplementation

``playerImplementation``
########################

+------------------------+---------------------------------------------------------------------------+
| **Option name**        | ``playerImplementation``                                                  |
+------------------------+---------------------------------------------------------------------------+
| Description            | Defines the "brand" of the embedded video player.                         |
+------------------------+---------------------------------------------------------------------------+
| Provided with          | * All TubePress distributions except TubePress for Wix                    |
+------------------------+---------------------------------------------------------------------------+
| Default value          | ``provider_based``                                                        |
+------------------------+---------------------------------------------------------------------------+
| Valid values           | ``provider_based``                                                        |
|                        |   Uses the provider's player (i.e. the standard YouTube player)           |
|                        | ``embedplus``                                                             |
|                        |   Plays videos with `EmbedPlus <http://www.embedplus.com/>`_              |
|                        | ``longtail``                                                              |
|                        |   Plays videos with `JW Player <http://www.jwplayer.com/>`_               |
+------------------------+---------------------------------------------------------------------------+
| Supported provider(s)  | YouTube                                                                   |
+------------------------+---------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress playerImplementation="longtail"]``                           |
+------------------------+---------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('playerImplementation="longtail"');`` |
+------------------------+---------------------------------------------------------------------------+

.. _option-playerLocation:

.. index::
   single: playerLocation; normal
   single: playerLocation
   single: playerLocation; popup
   single: playerLocation; youtube
   single: playerLocation; vimeo
   single: playerLocation; shadowbox
   single: playerLocation; jqmodal
   single: playerLocation; static
   single: playerLocation; solo
   single: playerLocation; fancybox
   single: playerLocation; tinybox
   single: Shadowbox.js
   single: jqModal
   single: TinyBox
   single: FancyBox

``playerLocation``
##################

+------------------------+------------------------------------------------------------------------------+
| **Option name**        | ``playerLocation``                                                           |
+------------------------+------------------------------------------------------------------------------+
| Description            | Defines the "location" of the embedded video player. This allows you |br|    |
|                        | to choose the location and effect of how the embedded videos play.           |
+------------------------+------------------------------------------------------------------------------+
| Provided with          | * All TubePress distributions, though availability varies                    |
+------------------------+------------------------------------------------------------------------------+
| Default value          | ``normal``                                                                   |
+------------------------+------------------------------------------------------------------------------+
| Valid values           | ``normal``                                                                   |
|                        |   Embedded player is placed above thumbnail gallery                          |
|                        | ``popup``                                                                    |
|                        |   Videos play in an HTML popup window                                        |
|                        | ``youtube``                                                                  |
|                        |   User is taken to the video's home on youtube.com for viewing.              |
|                        | ``vimeo``                                                                    |
|                        |   User is taken to the video's home on vimeo.com for viewing.                |
|                        | ``shadowbox``                                                                |
|                        |   Video plays in a modal window with `Shadowbox.js`_                         |
|                        | ``jqmodal``                                                                  |
|                        |   Video plays in a modal window with `jqModal`_                              |
|                        | ``solo``                                                                     |
|                        |   Page refreshes, and video player replaces the thumbnail gallery            |
|                        | ``static``                                                                   |
|                        |   Like ``normal``, but each thumbnail click triggers a page refresh          |
|                        | ``tinybox``                                                                  |
|                        |   Video plays in a modal window with `TinyBox`_. Not available in free |br|  |
|                        |   WordPress plugin.                                                          |
|                        | ``fancybox``                                                                 |
|                        |   Video plays in a modal window with `Fancybox`_. Not available in free |br| |
|                        |   WordPress plugin.                                                          |
+------------------------+------------------------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                                            |
+------------------------+------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress playerLocation="popup"]``                                       |
+------------------------+------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('playerLocation="popup"');``             |
+------------------------+------------------------------------------------------------------------------+

.. _Shadowbox.js: http://www.shadowbox-js.com/
.. _jqModal: http://dev.iceburg.net/jquery/jqModal/
.. _TinyBox: http://www.scriptiny.com/2009/05/javascript-popup-box/
.. _Fancybox: http://fancybox.net/

.. _option-showInfo:

.. index::
   single: showInfo

``showInfo``
############

+------------------------+------------------------------------------------------------------------------+
| **Option name**        | ``showInfo``                                                                 |
+------------------------+------------------------------------------------------------------------------+
| Description            | Show or hide the video's title, description, and other meta information |br| |
|                        | on the embedded video itself before playback begins.                         |
+------------------------+------------------------------------------------------------------------------+
| Provided with          | * All TubePress distributions                                                |
+------------------------+------------------------------------------------------------------------------+
| Default value          | ``false``                                                                    |
+------------------------+------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                        |
+------------------------+------------------------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                                            |
+------------------------+------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress showInfo="true"]``                                              |
+------------------------+------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('showInfo="true');``                     |
+------------------------+------------------------------------------------------------------------------+

.. _option-orderBy:

.. index::
   single: orderBy
   single: orderBy; commentCount

``orderBy``
###########

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``orderBy``                                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Define the overall sort order of the video feed. This only applies, |br|                   |
|                        | obviously, to video galleries and not individual videos.                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | * All TubePress distributions                                                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``default``                                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``commentCount``                                                                           |
|                        |   Only applies to YouTube playlist galleries and selected Vimeo galleries. |br|            |
|                        |   Videos with more comments will be shown before others. [1]_                              |
|                        | ``default``                                                                                |
|                        |   TubePress chooses the "best" sort order for the video source. |br|                       |
|                        |   e.g. search-based galleries are sorted by ``relevance``, and |br|                        |
|                        |   user uploads are sorted by ``newest``.                                                   |
|                        | ``duration``                                                                               |
|                        |   Only applies to YouTube playlist galleries. Longest-running videos shown |br|            |
|                        |   first. [2]_                                                                              |
|                        | ``newest``                                                                                 |
|                        |   Newest videos first. [1]_                                                                |
|                        | ``oldest``                                                                                 |
|                        |   Only applies to the following Vimeo galleries: ``vimeoUploadedBy``, |br|                 |
|                        |   ``vimeoLikes``, ``vimeoAppearsIn``, ``vimeoSearch``, |br|                                |
|                        |   ``vimeoCreditedTo``, ``vimeoGroup``. [3]_                                                |
|                        | ``position``                                                                               |
|                        |   Only applies to YouTube playlist galleries. Videos will be shown in the order in |br|    |
|                        |   which they appear in the playlist. [2]_                                                  |
|                        | ``random``                                                                                 |
|                        |   Only applies to Vimeo group-based galleries (``vimeoGroup``). Retrieves videos |br|      |
|                        |   in a random order. [4]_                                                                  |
|                        | ``rating``                                                                                 |
|                        |   Highest-rated videos first. [1]_                                                         |
|                        | ``relevance``                                                                              |
|                        |   Only applies to search-based galleries. Videos with the highest relevance |br|           |
|                        |   to the search terms will be shown first. [5]_                                            |
|                        | ``reversedPosition``                                                                       |
|                        |   Only applies to YouTube playlist galleries. Videos will be shown in the reverse |br|     |
|                        |   order of the ``position`` sort order. [2]_                                               |
|                        | ``title``                                                                                  |
|                        |   Only applies to YouTube playlist galleries. Videos will be shown in |br|                 |
|                        |   alphabetical order of their titles. [2]_                                                 |
|                        | ``viewCount``                                                                              |
|                        |   Most-viewed videos first. [1]_                                                           |
+------------------------+--------------------------------------------------------------------------------------------+
| Supported provider(s)  | Vimeo and YouTube                                                                          |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress orderBy="newest"]``                                                           |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('orderBy="newest"');``                                 |
+------------------------+--------------------------------------------------------------------------------------------+

.. |br| raw:: html

  <br />

.. rubric:: Footnotes

.. [1] `YouTube documentation <https://developers.google.com/youtube/2.0/reference#orderbysp>`_. Vimeo documentation
       for `search <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getByTag>`_,
       `user uploads <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getUploaded>`_,
       `user likes <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getLikes>`_,
       `user appears in <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getAppearsIn>`_,
       `credited to <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getAll>`_,
       and `groups <https://developer.vimeo.com/apis/advanced/methods/vimeo.groups.getVideos>`_.
.. [2] `YouTube documentation <https://developers.google.com/youtube/2.0/reference#orderbysp>`_.
.. [3] Vimeo documentation for `search <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getByTag>`_,
       `user uploads <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getUploaded>`_,
       `user likes <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getLikes>`_,
       `user appears in <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getAppearsIn>`_,
       `credited to <https://developer.vimeo.com/apis/advanced/methods/vimeo.videos.getAll>`_,
       and `groups <https://developer.vimeo.com/apis/advanced/methods/vimeo.groups.getVideos>`_.
.. [4] `Vimeo documentation <https://developer.vimeo.com/apis/advanced/methods/vimeo.groups.getVideos>`_.
.. [5] `YouTube documentation <https://developers.google.com/youtube/2.0/reference#orderbysp>`_.
       `Vimeo documentation <https://developers.google.com/youtube/2.0/reference#orderbysp>`_.