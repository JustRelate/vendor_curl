Solaris + Linux
---------------

  Sourcen geladen von http://curl.haxx.se/download.html

Dann

Linux:
./configure --prefix=/tmp/curl --enable-http --enable-ftp --enable-ipv6 --enable-crypto-auth --with-ssl=/usr/local/ssl/ --disable-static
(unter /usr/local/ssl liegt ein selbstgerolltes openssl-0.9.7i)

Solaris:
./configure --prefix=/tmp/curl --enable-http --enable-ftp --enable-ipv6 --enable-crypto-auth --with-ssl --disable-static

und

make
make install

Anschlieﬂend bin, lib/libcurl.so.3 und include/curl/ nach External/...
verschoben.  lib/lubcurl.so.3 dann in lib/libcurl.so umbenannt.

Windows
-------

  Binary geladen von http://curl.haxx.se/download.html.
  libcurl.dll in libcurl-3.dll umbenennen.

  Zusaetzlich auch von dieser Seite das "OpenSSL binary package" fuer Windows runterladen.
  Es enthaelt die benoetigten Libs libeay32.dll und libssl32.dll.
