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

