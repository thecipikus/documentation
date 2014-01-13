TubePress uses `Ajax <http://en.wikipedia.org/wiki/Ajax_(programming)>`_ extensively in the browser - e.g. to
asynchronously load the video player whenever a user clicks a thumbnail. By virtue of this, TubePress is forced
to adhere to the `same origin policy <http://en.wikipedia.org/wiki/Same_origin_policy>`_ of JavaScript. The same origin
policy should be embraced - at least until the Internet settles on
a `new policy <http://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_ - as its a crucial guard against malicious
sites.

However, this means that a small domain misconfiguration can lead to a broken/misbehaving TubePress installation.

As an example, say that you have a domain ``ehough.com`` and are serving a web site at this address;
loading up ``http://ehough.com`` works normally for your users, and TubePress detects that ``ehough.com`` is the domain
that it will use. But you *also* have the site available (without HTTP redirects) via ``http://www.ehough.com``.
Users that access the site via the ``www.ehough.com`` domain will experience a
broken TubePress installation, as TubePress will attempt to make a cross-domain Ajax request to ``ehough.com``.

To diagnose if this if your problem, use the following procedure:

  1. Using Firefox, navigate to a page with a TubePress gallery
  2. Open up Firebug
  3. Open Firebug's "Console" tab
  4. Click on any TubePress thumbnail. You should see a new XHR request show up as TubePress performs its Ajax request.

     .. image:: ../_shared/troubleshooting/images/cross_domain_xhr.png

  5. Expand this request (using the expand icon on the left) to view the results. You should see a small/medium
     `JSON <http://www.json.org/>`_ result. If you see **anything** else here, or nothing at all, then something is wrong

     .. image:: ../_shared/troubleshooting/images/cross_domain_xhr_result.png

To fix this issue, `Google recommends <http://support.google.com/webmasters/bin/answer.py?hl=en&answer=66359>`_ to
choose a "preferred domain" and stick with it. Here are some guidelines on how to achieve this:

 * Use HTTP 301 redirects ("RedirectPermanent") in your .htaccess file to smartly redirect users to your preferred domain.
   * In Apache, you can do this with an .htaccess file.
   * In IIS, you can do this through the administrative console.
 * WordPress users should make sure that both their "Site Address" and "WordPress Address" match their preferred domain
   (you can set these at ``WP Admin > Settings > General``)
 * If you use TubePress Pro in a PHP environment, make sure that the domain you set with ``TubePressPro::setBaseUrl()``
   matches your preferred domain
