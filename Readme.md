## Custom DarwinPorts local sources

>
$ mkdir ~/DarwinPorts
>
$ cd ~/DarwinPorts
>
$ git clone git://github.com/liut/DarwinPorts-local-sources.git local-sources
>
$ sudo vim /opt/local/etc/macports/sources.conf


	#  To get the ports tree from the master MacPorts server in California, USA use:
	#      rsync://rsync.macports.org/release/ports/
	#  To get it from the mirror in Trondheim, Norway use:
	#      rsync://trd.no.rsync.macports.org/release/ports/
	#  A current list of mirrors is available at http://trac.macports.org/wiki/Mirrors

	## add local sources
	file:///Users/liut/DarwinPorts/local-sources

	rsync://rsync.macports.org/release/ports/ [default]



### current ports

* php5-fpm: set fpm as default variant

>	sudo port -v install php5-fpm +mysqlnd+zip

* php5-taint: http://pecl.php.net/package/taint/

>	sudo port -v install php5-taint

* php5-yaf: http://pecl.php.net/package/yaf/

>	sudo port -v install php5-yaf
