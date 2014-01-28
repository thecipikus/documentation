YouTube Options
===============

.. contents:: On This Page
   :local:

.. _youtube-gallery-sources:

Gallery Sources
---------------

.. contents:: General Options
   :local:

.. _mode-playlist:

.. index::
   single: gallery source; playlist

``playlist``
#################################

+------------------------+--------------------------------------------------------------------------------------------+
| **Gallery source**     | ``playlist``                                                                               |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Videos from a YouTube playlist. The playlist is defined by the value |br|                  |
|                        | you supply to the ``playlistValue`` attribute.                                             |
+------------------------+--------------------------------------------------------------------------------------------+
| Notes                  | Limited to 200 videos. Currently, only public playlists can |br|                           |
|                        | be shown with TubePress.                                                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="playlist" playlistValue="6813408AE8D50E6F"]``                           |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="playlist" playlistValue="6813408AE8D50E6F"');`` |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/reference#Playlist_feed>`_          |
+------------------------+--------------------------------------------------------------------------------------------+

.. _mode-favorites:

.. index::
   single: gallery source; favorites

``favorites``
#############

+------------------------+--------------------------------------------------------------------------------------------+
| **Gallery source**     | ``favorites``                                                                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | "Favorite" videos of a YouTube user. The YouTube user is defined by the value |br|         |
|                        | you supply to the ``favoritesValue`` attribute.                                            |
+------------------------+--------------------------------------------------------------------------------------------+
| Notes                  | Limited to 50 videos.                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="favorites" favoritesValue="3hough"]``                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="favorites" favoritesValue="3hough"');``         |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/reference#User_favorites_feed>`_    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _mode-tag:

.. index::
   single: gallery source; tag

``tag``
#######

+------------------------+-----------------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``tag``                                                                                                   |
+------------------------+-----------------------------------------------------------------------------------------------------------+
| Description            | YouTube videos matching a search term. Supply space-separated search |br|                                 |
|                        | terms to the tagValue attribute. To search for an exact phrase, |br|                                      |
|                        | enclose the phrase in double quotes. Use the pipe character (``|``) to |br|                               |
|                        | indicate a boolean OR, and the minus character (``-``) to exclude a term.                                 |
+------------------------+-----------------------------------------------------------------------------------------------------------+
| Notes                  | Limited to approximately 1000 videos.                                                                     |
+------------------------+-----------------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="tag" tagValue='"pittsburgh steelers" highlights -playoffs']``                          |
+------------------------+-----------------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="tag" tagValue='"pittsburgh steelers" -highlights playoffs');`` |
+------------------------+-----------------------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/reference#Searching_for_videos>`_                  |
+------------------------+-----------------------------------------------------------------------------------------------------------+

.. _mode-user:

.. index::
   single: gallery source; user

``user``
########

+------------------------+----------------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``user``                                                                                                 |
+------------------------+----------------------------------------------------------------------------------------------------------+
| Description            | YouTube videos uploaded by a specific YouTube user. The YouTube user is |br|                             |
|                        | defined by the value you supply to the userValue attribute.                                              |
+------------------------+----------------------------------------------------------------------------------------------------------+
| Notes                  | Limited to 1000 videos.                                                                                  |
+------------------------+----------------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="user" userValue="3hough"]``                                                           |
+------------------------+----------------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="user" userValue="3hough"');``                                 |
+------------------------+----------------------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/developers_guide_protocol#User_Uploaded_Videos>`_ |
+------------------------+----------------------------------------------------------------------------------------------------------+

.. _mode-youtubeMostPopular:

.. index::
   single: gallery source; youtubeMostPopular

``youtubeMostPopular``
######################

+------------------------+--------------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``youtubeMostPopular``                                                                                 |
+------------------------+--------------------------------------------------------------------------------------------------------+
| Description            | The most popular YouTube videos, selected using a YouTube algorithm |br|                               |
|                        | that combines many different signals to determine overall popularity. |br|                             |
|                        | You can supply ``all_time`` or ``today`` to the ``youtubeMostPopularValue`` |br|                       |
|                        | option to control the time frame of the results.                                                       |
+------------------------+--------------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="youtubeMostPopular" youtubeMostPopularValue="all_time"]``                           |
+------------------------+--------------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="youtubeMostPopular" youtubeMostPopularValue="all_time"');`` |
+------------------------+--------------------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/reference#Standard_feeds>`_                     |
+------------------------+--------------------------------------------------------------------------------------------------------+

.. _mode-youtubeRelated:

.. index::
   single: gallery source; youtubeRelated

``youtubeRelated``
##################

+------------------------+---------------------------------------------------------------------------------------------------+
| **Gallery source**     | ``youtubeRelated``                                                                                |
+------------------------+---------------------------------------------------------------------------------------------------+
| Description            | YouTube videos related to a specific YouTube video. The target YouTube video is |br|              |
|                        | identified by the value supplied to the youtubeRelatedValue option.                               |
+------------------------+---------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress mode="youtubeRelated" youtubeRelatedValue="ZTUVgYoeN_b"]``                           |
+------------------------+---------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('mode="youtubeRelated" youtubeRelatedValue="ZTUVgYoeN_b"');`` |
+------------------------+---------------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/reference#Related_videos_feed>`_           |
+------------------------+---------------------------------------------------------------------------------------------------+

Embedded Video Player
---------------------

.. contents:: Embedded Video Player
   :local:

.. _option-autoHide:

.. index::
   single: video player; auto-hide YouTube controls

``autoHide``
#################################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``autoHide``                                                                               |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Automatically fade out elements of the video player after a few moments of playback.       |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``fadeOnlyProgressBar``                                                                    |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``fadeBoth``                                                                               |
|                        |   Fade both the progress bar and the video controls                                        |
|                        | ``fadeNone``                                                                               |
|                        |   Always show both the progress bar and the video controls                                 |
|                        | ``fadeOnlyProgressBar``                                                                    |
|                        |   Fade only the progress bar, but continue to show the video controls.                     |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress autoHide="fadeNone"]``                                                        |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('autoHide="fadeNone"');``                              |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-fullscreen:

.. index::
   single: video player; fullscreen playback

``fullscreen``
##############

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``fullscreen``                                                                             |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Enable or disable the fullscreen playback option.                                          |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``true``                                                                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress fullscreen="false"]``                                                         |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('fullscreen="false"');``                               |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-modestBranding:

.. index::
   single: video player; YouTube modest branding

``modestBranding``
##################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``modestBranding``                                                                         |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | If enabled, hides the YouTube logo from the video controls area.                           |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``true``                                                                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress modestBranding="false"]``                                                     |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('modestBranding="false"');``                           |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-showRelated:

.. index::
   single: video player; related videos

``showRelated``
###############

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``showRelated``                                                                            |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Toggles display of related videos when playback finishes.                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``true``                                                                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress showRelated="false"]``                                                        |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('showRelated="false"');``                              |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-youtubeClosedCaptions:

.. index::
   single: video player; closed captions

``youtubeClosedCaptions``
#########################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``youtubeClosedCaptions``                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Show closed captions by default.                                                           |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress youtubeClosedCaptions="true"]``                                               |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('youtubeClosedCaptions="true"');``                     |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-youtubeDisableKeyboardControls:

.. index::
   single: video player; keyboard controls

``youtubeDisableKeyboardControls``
##################################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``youtubeDisableKeyboardControls``                                                         |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Disable all keyboard controls for the video.                                               |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress youtubeDisableKeyboardControls="true"]``                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('youtubeDisableKeyboardControls="true"');``            |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-youtubePlayerTheme:

.. index::
   single: video player; YouTube theme

``youtubePlayerTheme``
######################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``youtubePlayerTheme``                                                                     |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | The color theme of the video player .                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``dark``                                                                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``dark`` or ``light``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress youtubePlayerTheme="light"]``                                                 |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('youtubePlayerTheme="light"');``                       |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-youtubeShowAnnotations:

.. index::
   single: video player; annotations

``youtubeShowAnnotations``
##########################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``youtubeShowAnnotations``                                                                 |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Show video annotations by default.                                                         |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress youtubeShowAnnotations="true"]``                                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('youtubeShowAnnotations="true"');``                    |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-youtubeShowPlayerControls:

.. index::
   single: video player; showing controls

``youtubeShowPlayerControls``
#############################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``youtubeShowPlayerControls``                                                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Toggles display of the video controls.                                                     |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``showDelayed``                                                                            |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``hide``                                                                                   |
|                        |   Hide all video controls                                                                  |
|                        | ``showImmediate``                                                                          |
|                        |   Show the video controls. When the Flash player is used, Flash will load immediately.     |
|                        | ``showDelayed``                                                                            |
|                        |   Show the video controls. When the Flash player is used, Flash will |br|                  |
|                        |   load when video playback begins                                                          |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress youtubeShowPlayerControls="fadeNone"]``                                       |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('youtubeShowPlayerControls="fadeNone"');``             |
+------------------------+--------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/player_parameters>`_                    |
+------------------------+--------------------------------------------------------------------------------------------+

Video Feed
----------

.. contents:: Video Feed Options
   :local:

.. _option-developerKey:

.. index::
   single: options (by name); developerKey
   single: video feed; YouTube developer key

``developerKey``
################

+------------------------+-------------------------------------------------------------------------------------------------------------------+
| **Option name**        | ``developerKey``                                                                                                  |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Description            | YouTube API developer key. YouTube will use this developer |br|                                                   |
|                        | key for logging and debugging purposes if you experience a |br|                                                   |
|                        | service problem on their end.                                                                                     |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Provided with          | All downloadable TubePress distributions                                                                          |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Default value          | *hidden*                                                                                                          |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Valid values           | Any valid YouTube API key                                                                                         |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress developerKey="..."]``                                                                                |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('developerKey="..."');``                                                      |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/developers_guide_protocol_authentication#Authentication>`_ |
+------------------------+-------------------------------------------------------------------------------------------------------------------+

.. _option-embeddableOnly:

.. index::
   single: options (by name); embeddableOnly

``embeddableOnly``
##################

+------------------------+-------------------------------------------------------------------------------------------------------------------+
| **Option name**        | ``embeddableOnly``                                                                                                |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Description            | Some videos have embedding disabled. Enabling this option will |br|                                               |
|                        | exclude these videos from your galleries. Most users will never |br|                                              |
|                        | need to modify this option.                                                                                       |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Provided with          | All downloadable TubePress distributions                                                                          |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Default value          | ``true``                                                                                                          |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                                             |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress embeddableOnly="true"]``                                                                             |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('embeddableOnly="true"');``                                                   |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/reference#formatsp>`_                                      |
+------------------------+-------------------------------------------------------------------------------------------------------------------+

.. _option-filter_racy:

.. index::
   single: options (by name); filter_racy
   single: video feed; filtering restricted content

``filter_racy``
###############

+------------------------+-------------------------------------------------------------------------------------------------------------------+
| **Option name**        | ``filter_racy``                                                                                                   |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Description            | Filter out restricted content. YouTube performs the filtering |br|                                                |
|                        | much in the same manner as `SafeSearch Filtering for Google WebSearch`_.                                          |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Provided with          | All downloadable TubePress distributions                                                                          |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Default value          | ``moderate``                                                                                                      |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Valid values           | ``none``                                                                                                          |
|                        |   YouTube will not perform any filtering.                                                                         |
|                        | ``moderate``                                                                                                      |
|                        |   YouTube will filter some videos.                                                                                |
|                        | ``strict``                                                                                                        |
|                        |   YouTube will try to exclude all restricted videos.                                                              |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress filter_racy="strict"]``                                                                              |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('filter_racy="strict"');``                                                    |
+------------------------+-------------------------------------------------------------------------------------------------------------------+
| YouTube documentation  | `Click here <https://developers.google.com/youtube/2.0/reference#safeSearchsp>`_                                  |
+------------------------+-------------------------------------------------------------------------------------------------------------------+

.. _SafeSearch Filtering for Google WebSearch: http://www.google.com/support/bin/static.py?page=searchguides.html&ctx=preferences&hl=en

Video Meta Display
------------------

.. _option-rating:

.. index::
   single: options (by name); rating

``rating``
##########

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``rating``                                                                                 |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Toggle display of the video's average rating.                                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress rating="true"]``                                                              |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('rating="true"');``                                    |
+------------------------+--------------------------------------------------------------------------------------------+

.. _option-ratings:

.. index::
   single: options (by name); ratings

``ratings``
###########

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``ratings``                                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Toggle display of the number of times the video has been rated.                            |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | All TubePress distributions                                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress ratings="true"]``                                                             |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('ratings="true"');``                                   |
+------------------------+--------------------------------------------------------------------------------------------+

Thumbnails
----------

.. _option-youtubeHideBlackBars:

.. index::
   single: options (by name); youtubeHideBlackBars
   single: thumbnails; black bars

``youtubeHideBlackBars``
########################

+------------------------+--------------------------------------------------------------------------------------------+
| **Option name**        | ``youtubeHideBlackBars``                                                                   |
+------------------------+--------------------------------------------------------------------------------------------+
| Description            | Hides the "black bars" on most YouTube thumbnails.                                         |
+------------------------+--------------------------------------------------------------------------------------------+
| Provided with          | :doc:`../../manual/add-ons/youtube-black-bars-remover/index`                               |
+------------------------+--------------------------------------------------------------------------------------------+
| Default value          | ``false``                                                                                  |
+------------------------+--------------------------------------------------------------------------------------------+
| Valid values           | ``true`` or ``false``                                                                      |
+------------------------+--------------------------------------------------------------------------------------------+
| Shortcode example      | ``[tubepress youtubeHideBlackBars="true"]``                                                |
+------------------------+--------------------------------------------------------------------------------------------+
| Standalone PHP example | ``TubePressPro::getHtmlForShortcode('youtubeHideBlackBars="true"');``                      |
+------------------------+--------------------------------------------------------------------------------------------+

.. |br| raw:: html

  <br />
