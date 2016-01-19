Zabbix template observes Linux Software RAID (md)
==================

Description
-----------------
- simple installation - based on /proc/mdstat and zabbix regexp item without Low Level Discovery;
- not use any additional files/actions on monitored server(s), only zabbix agent is needed;
- correctly worked on every linux OS even if linux don't have raid.
- any raid numbers are available;
- show the problem with raid without detalization;
- checked status of raids once an hour

TO DO list
------

- try to show detailed info about raid(s) problem which
- number of problem (problem on 1, 2, 3 raids)


Installation
----------------

Import Zabbix template and add template to the monitored servers.
You can just link the template to standard zabbix "Template OS Linux" and all servers worked under it will be checked on software RAID issues.

Referrence:
-------

- https://www.kernel.org/doc/Documentation/md.txt
