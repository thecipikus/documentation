Single Video Embeds
^^^^^^^^^^^^^^^^^^^

Embedding a single video into a website is easy and common. Nearly every video provider includes an "embed" option
for each video that provides an HTML ``<iframe>`` that can be added to any website. If you're reading this, you've
probably done this countless times.

TubePress improves the embedding process by

 1. Abstracting away the HTML. No need to copy and paste a long and complicated ``<iframe>`` snippet.
 2. Allowing you to control the embedded video player (e.g. colors, behavior, size, etc).
 3. Bringing in all of the video's meta information (length, description, author, keywords, etc). You can even have
    fine-grained control over how the meta information is presented; it's just simple HTML.

.. image:: ../_images/feature/single-video-embed.png

To embed a single video with TubePress, you simply need to give TubePress the ID of the video you'd like to embed. For
instance, if you want to embed the YouTube video with ID J51kfduN5aA, you would use use the following shortcode:

.. code-block:: php

  [tubepress video="J51kfduN5aA"]