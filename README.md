# Chef Cookbook for Zabbix on Windows

Master branch: [![Build Status](https://secure.travis-ci.org/thomasvincent/zabbix_windows_chef)](https://secure.travis-ci.org/thomasvincent/zabbix_windows_chef)
[![Inline docs](http://inch-ci.org/github/thomasvincent/zabbix_windows_chef.png)](http://inch-ci.org/github/thomasvincent/zabbix_windows_chef) [![Stories in Ready](https://badge.waffle.io/thomasvincent/zabbix_windows_chef.png?label=ready&title=Ready)](https://waffle.io/thomasvincent/zabbix_windows_chef)

=======
Description
===========
Install the Zabbix agent on Windows machines.


Requirements
============
A Zabbix server is required for this to do anything useful.

Originally, I intended this to be added to Nacer Laradji's [Zabbix Cookbook](http://community.opscode.com/cookbooks/zabbix) ([github](https://github.com/laradji/zabbix)), but there were significant problems making it work this way.  (I believe that this is because there are problems in the dependancy chain that prevent this from working directly from the Zabbix cookbook; those cookbooks do not support the Windows platform.)

So, I present to you, a standalone recipe for installing the Zabbix Agent on your Windows hosts.


Attributes
==========
I am attempting to leverage the (mostly) standard attributes that I have included.

At this time, the actual files placed are version 2.2.9 and have been placed in the recipe manually.  Later I may have them fetched as remote_file with respect to the version


Usage
=====
Simply add the "Zabbix\_windows" recipe to a windows machine after establishing your Zabbix server and setting the Attributes as appropriate to your environment.


## Supported Platforms

* Windows 2008
* Windows 2012

## License and Authors

- Author:: Thomas Vincent (thomasvincent@gmail.com)
- Original author who @thomasvincent adopted on Supermarket from Author:: [H. "Waldo" Grunenwald][@gwaldo]
- Updated:: Evan Montgomery-Recht (montge@mianetworks.net)
