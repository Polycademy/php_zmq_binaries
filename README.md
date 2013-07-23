PHP ZMQ BInaries
=================

Finding ZMQ binaries for PHP on Windows is difficult, the official site doesn't work. So I decided to make a repo of the updated ones I find.

Put the libzmq.dll into your PHP's binary directory.
Put the php_zmq.dll (the appropriate one, try each of them) into your php/ext directory.
Write this into your php.ini (cli and http):

```
[ZMQ]
extension=php_zmq.dll
```

Install the ZMQ client, either the one I bundled or download one from the main site.
Restart and test out the modules with "php -m" in the CLI.

Also refer to these sites for new releases:

1. https://github.com/mkoppanen/php-zmq
2. https://github.com/mkoppanen/php-zmq/wiki
3. https://github.com/WPN-XM/WPN-XM/issues/82
4. http://stackoverflow.com/questions/6742773/zeromq-php-extension-for-windows