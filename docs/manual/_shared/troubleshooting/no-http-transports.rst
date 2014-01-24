If you get an error message from TubePress that looks like

  No HTTP transports could execute GET to ...

it means that you PHP installation has been configured to block nearly all network operations. This is often
done as a security measure to prevent malicious PHP scripts from "phoning home."

TubePress needs to open HTTP connections to talk to video providers like YouTube or Vimeo. Under the hood, TubePress
uses the `shortstop HTTP client <https://github.com/ehough/shortstop>`_, which attempts to use the following PHP mechanisms:

 * `cURL extension <http://php.net/manual/book.curl.php>`_
 * `HTTP extension <http://php.net/manual/book.http.php>`_
 * `fsockopen() <http://php.net/manual/function.fsockopen.php>`_
 * `fopen() <http://php.net/manual/function.fopen.php>`_
 * `Streams extension <http://www.php.net/manual/book.stream.php>`_

So the solution is to allow TubePress to use one or more of these mechanisms. You, or your hosting provider, must
perform **at least one** of the following:

 * Install and allow the `cURL extension <http://php.net/manual/book.curl.php>`_
 * Install and allow the `HTTP extension <http://php.net/manual/book.http.php>`_
 * Remove ``fsockopen()`` from the list of `disabled functions <http://php.net/manual/ini.core.php#ini.disable-functions>`_
 * Remove ``fopen()`` from the list of `disabled functions <http://php.net/manual/ini.core.php#ini.disable-functions>`_
