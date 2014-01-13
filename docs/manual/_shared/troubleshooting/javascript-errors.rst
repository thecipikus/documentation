If your website has JavaScript errors, they can prevent TubePress from operating correctly.

TubePress expects your page to load cleanly; i.e. there should be no JavaScript errors caused by other scripts,
plugins, themes, etc. The reason is that TubePress relies on jQuery's `ready() <http://api.jquery.com/ready/>`_
function, which can get interrupted if other scripts cause errors.

To diagnose if this is your problem, use the following procedure:

 1. Using Firefox, navigate to a page with a TubePress gallery
 2. Open up Firebug.
 3. Open Firebug's "Console" tab
 4. Refresh the page.
 5. Check Firebug's console for JavaScript errors

The image below shows what JavaScript errors look like in Firebug.

.. image:: ../_shared/troubleshooting/images/js-errors.png

**The resolution is always to fix the script causing the error**. Usually this entails identifying which component of your
site (script, plugin, etc) is causing the error. Unfortunately since sites can get extremely complicated, there's
no "one size fits all" solution.

Typically by hovering over the JavaScript errors in Firebug, you can pinpoint which JavaScript file is causing the trouble.