Vimeo All Access
==========================

.. contents:: On This Page
   :local:

.. _vimeo-all-access-intro:

Introduction
--------------

This TubePress add-on provides TubePress with enhanced access to your
Vimeo `Plus <https://vimeo.com/plus>`_ or `PRO <https://vimeo.com/pro>`_ account, thus allowing TubePress to work
with `private Vimeo videos <https://vimeo.com/help/faq/managing-your-videos/privacy-settings>`_.

This is particularly useful if you'd like to hide your videos from display on vimeo.com and *only* show them on
your TubePress-powered site. To make a video private, choose the last radio icon in the privacy settings for the video as
shown below:

.. image:: images/vimeo-privacy-settings.png

.. _vimeo-all-access-manuals:

Manuals
----------

.. _vimeo-all-access-manual-wordpress:

TubePress for WordPress
^^^^^^^^^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/42-youtube-black-bars-remover/>`_.
 2. Unzip the file you downloaded (``vimeo-all-access_x_y_z.zip``) into the ``add-ons`` subdirectory of your
    :ref:`TubePress Content Directory <wordpress-tubepress-content-directory>`.
 3. Follow the instructions on this page under :ref:`vimeo-all-access-obtain-credentials`.
 4. Supply your newly-obtained credentials TubePress at ``WP Admin > Settings > TubePress > Feed``. On this tab you will see two new text boxes for this add-on:

.. image:: images/wordpress-settings.png

.. _vimeo-all-access-manual-php:

TubePress for PHP
^^^^^^^^^^^^^^^^^^^^^

 1. Purchase and download this add-on from `the TubePress Marketplace <http://community.tubepress.com/files/file/42-youtube-black-bars-remover/>`_.
 2. Unzip the file you downloaded (``vimeo-all-access_x_y_z.zip``) into the ``add-ons`` subdirectory of your
    :ref:`TubePress Content Directory <standalone-tubepress-content-directory>`.
 3. Follow the instructions on this page under :ref:`vimeo-all-access-obtain-credentials`.

.. _vimeo-all-access-manual-cloud:

Cloud-based TubePress Installations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Users of cloud-based TubePress installations (e.g. TubePress Express, TubePress for Wix) should follow these instructions.

In order to use TubePress with Vimeo, you are required to obtain a "consumer key" and "consumer secret"
from Vimeo. This is a one-time setup required by Vimeo. Thankfully it's easy to create these credentials and supply them to
TubePress.

 1. `Log in to Vimeo <http://vimeo.com/log_in>`_, if you haven't already.
 2. `Click here <https://developer.vimeo.com/apps/new>`_ to create a new Vimeo app. You can fill in anything
    for the fields. Below is a sample form that's filled out. Then click the `Create App` button.

    .. image:: ../../_shared/installation/images/vimeo_new_app.png

 3. Make a note of the "Client ID" and "Client secret" of your new app. See the red box below for an idea
    of what it should look like.

    .. image:: ../../_shared/installation/images/vimeo_new_keys.png

 4. Follow the instructions on this page under :ref:`vimeo-all-access-obtain-credentials`.

.. _vimeo-all-access-obtain-credentials:

Obtaining API Credentials
----------------------------

You will need to supply an additional set of Vimeo API credentials to TubePress: an "Access Token" with a corresponding
"Access Token Secret". This is a one-time step for this add-on.

.. warning:: It is extremely important to never publicly divulge these credentials.

..

 1. Visit https://developer.vimeo.com/apps. You should see a list of any Vimeo apps that you have created. Click on the
    app that you are using for TubePress.
 2. At the bottom of the page, you will see a box containing your Access Token and Access Token Secret:

    .. image:: images/access-token-and-secret.png