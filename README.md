zichan - A lightweight and full featured PHP textboard.
========================================================

About
------------
Zichan is a free light-weight, fast, highly configurable and user-friendly
textboard software package fork of vichan. It is written in PHP and has few dependencies.

The vichan documentation can be found on the [wiki](https://github.com/vichan-devel/vichan/wiki) and will work . (feel free to contribute)

History
------------
Zichan is a fork of [vichan](http://github.com/vichan-devel/vichan) designed primarily for textboard use. It is highly experimental and may contain leftovers.

### Maintainer timeline
1. The zichan fork is created and maintained by an anonymous developer
2. Community support for vichan by [@basedgentoo](https://github.com/basedgentoo), and [@RealAngeleno](https://github.com/RealAngeleno) - vichan
3. Development Commission lead by [@basedgentoo](https://github.com/basedgentoo), [@kuz-sysadmin](https://github.com/kuz-sysadmin), and [@RealAngeleno](https://github.com/RealAngeleno). (2023 - 2023 )
4. [@h00j](https://github.com/h00j) (2021 - ???)
5. [@ctrlcctrlv](https://github.com/ctrlcctrlv) (2017 - 2021)
6. [@czaks](https://github.com/czaks) (2014 - 2017) (The author of vichan fork)
7. [@savetheinternet](https://github.com/savetheinternet) (2010 - 2014) (The creator of Tinyboard)

Requirements
------------
1.	PHP >= 5.4 (we still try to keep compatibility with php 5.3 as much as possible)
        PHP 7.0 is explicitly supported. PHP 7.2 works as well, but may cause as yet unreported bugs.
2.	MySQL/MariaDB server
3.	[mbstring](http://www.php.net/manual/en/mbstring.installation.php) 
4.	[PHP GD](http://www.php.net/manual/en/intro.image.php)
5.	[PHP PDO](http://www.php.net/manual/en/intro.pdo.php)
6.	A Unix-like OS, preferrably FreeBSD or GNU/Linux

We try to make sure vichan is compatible with all major web servers. vichan does not include an Apache `.htaccess` file nor does it need one.

### Recommended
1.	MySQL/MariaDB server >= 5.5.3
2.	~~[APC (Alternative PHP Cache)](http://php.net/manual/en/book.apc.php)~~,
	[APCu (Alternative PHP Cache)](http://php.net/manual/en/book.apcu.php),
	[XCache](http://xcache.lighttpd.net/),
	[Memcached](http://www.php.net/manual/en/intro.memcached.php) or
	[Redis](https://redis.io/docs/about/)

Contributing
------------
You can contribute to zichan by:
*	Developing patches/improvements/translations and using GitHub to submit pull requests
*	Providing feedback and suggestions
*	Writing/editing documentation

Installation
-------------
1.	Download and extract zichan to your web directory or get the latest
	development version with:

        git clone git://github.com/vichan-devel/vichan.git

2.	run ```composer install``` inside the directory	
3.	Navigate to ```install.php``` in your web browser and follow the
	prompts.
4.	vichan should now be installed. Log in to ```mod.php``` with the
	default username and password combination: **admin / password**.

Please remember to change the administrator account password.

See also: [Configuration Basics](https://github.com/vichan-devel/vichan/wiki/config).

Support
--------
vichan is still beta software -- there are bound to be bugs. If you find a
bug, please report it.

CLI tools
-----------------
There are a few command line interface tools, based on Tinyboard-Tools. These need
to be launched from a Unix shell account (SSH, or something). They are located in a ```tools/```
directory.

You actually don't need these tools for your imageboard functioning, they are aimed
at the power users. You won't be able to run these from shared hosting accounts
(i.e. all free web servers).

vichan API
----------
vichan provides by default a 4chan-compatible JSON API. For documentation on this, see:
https://github.com/vichan-devel/vichan-API/ .
