.. _standalone-basic-usage:

Using TubePress in PHP
============================

.. contents:: On This Page
   :local:

.. _basic-standalone-configuration:

Add TubePress to any PHP Page
-----------------------------------

Follow these instructions to use TubePress Pro in a standalone PHP environment. You can integrate TubePress into any
PHP page on your site. For demonstration purposes, we will use the very simple PHP/HTML file show below. Feel
free to create this file, or extrapolate the concepts into your existing PHP. As you can see by the highlighted
lines of code, there are **four** key points.

.. code-block:: php
   :linenos:
   :emphasize-lines: 3,5,12,17

   <?php

       include "/var/www/html/myblog.com/lib/tubepress_pro_x_y_z/src/main/php/classes/TubePressPro.php";

       TubePressPro::setBaseUrl("http://myblog.com/lib/tubepress_pro_x_y_z");
   ?>

   <html>
       <head>
           <title>TubePress Pro</title>

           <?php print TubePressPro::getHtmlForHead(true); ?>

       </head>
       <body>

           <?php print TubePressPro::getHtmlForShortcode('mode="tag" tagValue="pittsburgh steelers" resultsPerPage="3"'); ?>

       </body>
   </html>

..

 1. Include the TubePress Pro class definition (``TubePressPro.php``). An absolute path works best.
 2. Call ``TubePressPro::setBaseUrl()`` with the *web-accessible* URL of your TubePress Pro installation.
 3. Include this statement in the HTML head of your document to print out the required TubePress CSS and JavaScript libraries. It takes a single parameter which indicates whether or not to include jQuery. If you are already including jQuery in your document, use ``false`` for this parameter.
 4. The ``getHtmlForShortcode()`` function takes a single string parameter which is any valid TubePress shortcode. It returns the HTML output of TubePress. You may repeat this function call as many times as you like.

Changing the Default Language
-----------------------------

.. include:: ../_shared/usage/i18n_intro.rst

You can tell TubePress which language to use via the ``lang`` option. Simply supply your two-letter
`language <http://www.gnu.org/software/gettext/manual/gettext.html#Language-Codes>`_
and `country <http://www.gnu.org/software/gettext/manual/gettext.html#Country-Codes>`_ code:

.. code-block:: php

   <?php

   TubePressPro::getHtmlForShortcode('lang="it_IT"');