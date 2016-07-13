# w3af SlackBuilds

This repository provides all the required SlackBuilds to build _w3af_ on
Slackware Linux.  It aims to be compatible with _slackrepo_ for testing
purposes.  The end goal is to incorporate _w3af_ into SlackBuilds.org
for distribution.

### Build

1.  Install Slackware64-current in a virtual machine
2.  Build the latest git revision of slackrepo
3.  Install slackrepo in the fresh VM of Slackware
4.  Clone the w3af-sbo repository into /home/$USER
5.  Copy /etc/slackrepo/SBo to /etc/slackrepo/w3af-sbo
6.  Copy slackrepo_w3af-sbo.conf to /etc/slackrepo from w3af-sbo git
7.  Run; "slackrepo update"
8.  Run: "slackrepo build w3af"

### Installation

1.  Packages will be located in /var/lib/slackrepo/w3af-sbo/packages/
2.  Run installpkg
``` bash
installpkg /var/lib/slackrepo/w3af-sbo/packages/*/*/*/*/*.t?z 
```

3.  Run w3af_console or w3af_gui to use w3af

### Removal

Be certain you run the correct commmand.  I am not responsible for any
damages to your operating system.

*  Run removepkg on the _same_ files you installed
``` bash
removepkg /var/lib/slackrepo/w3af-sbo/packages/*/*/*/*/*.t?z
```

##### Links
* [w3af](https://github.com/andresriancho/w3af)
* [Slackware](http://www.slackware.com/)
* [SlackBuilds.org](http://www.slackbuilds.org)
* [slackrepo](https://idlemoor.github.io/slackrepo/index.html)
