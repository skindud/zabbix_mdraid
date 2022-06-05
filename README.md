Zabbix template observes Linux Software RAID (md)
==================


<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

[![GitHub Super-Linter][linter-shield]][linter-url]

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

Referrences
-------

- <https://www.kernel.org/doc/Documentation/md.txt>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/skindud/zabbix_mdraid.svg?style=for-the-badge
[contributors-url]: https://github.com/skindud/zabbix_mdraid/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/skindud/zabbix_mdraid.svg?style=for-the-badge
[forks-url]: https://github.com/skindud/zabbix_mdraid/network/members
[stars-shield]: https://img.shields.io/github/stars/skindud/zabbix_mdraid.svg?style=for-the-badge
[stars-url]: https://github.com/skindud/zabbix_mdraid/stargazers
[issues-shield]: https://img.shields.io/github/issues/skindud/zabbix_mdraid.svg?style=for-the-badge
[issues-url]: https://github.com/skindud/zabbix_mdraid/issues
[license-shield]: https://img.shields.io/github/license/skindud/zabbix_mdraid.svg?style=for-the-badge
[license-url]: https://github.com/skindud/zabbix_mdraid/blob/master/LICENSE.txt

[linter-shield]: https://github.com/skindud/zabbix_mdraid/workflows/Lint%20Code%20Base/badge.svg
[linter-url]: https://github.com/skindud/zabbix_mdraid/actions
