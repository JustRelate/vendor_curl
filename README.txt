Solaris + Linux
---------------

  Sourcen geladen von http://curl.haxx.se/download.html

Dann

Linux:
./configure --prefix=/tmp/curl --disable-ldap --without-libidn --enable-http --enable-ftp --enable-ipv6 --enable-crypto-auth --with-ssl=<External>/openssl/<OS>/<version> --disable-shared

(ggf. ist LDFLAGS=-ldl nötig, wenn configure die packageconfig von openssl
nicht richtig ausliest)

und

make
make install

Anschließend bin, lib und include nach External/curl/… verschoben.

Windows
-------

  Binary geladen von http://curl.haxx.se/download.html.
  libcurl.dll in libcurl-3.dll umbenennen.

  Zusaetzlich auch von dieser Seite das "OpenSSL binary package" fuer Windows runterladen.
  Es enthaelt die benoetigten Libs libeay32.dll und libssl32.dll.
