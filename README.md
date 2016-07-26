Ansible Role for Memcached
==========================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-memcached.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-memcached)
[![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-memcached.svg)](https://github.com/pantarei/ansible-role-memcached)
[![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-memcached.svg)](https://github.com/pantarei/ansible-role-memcached/blob/master/LICENSE)

Ansible Role for Memcached Installation.

Requirements
------------

This role require Ansible 2.0 or higher.

This role was designed for Ubuntu Server 14.04 LTS and Ubuntu Server 16.04 LTS.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>parameter</th>
<th>required</th>
<th>default</th>
<th>choices</th>
<th>comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>memcached_connections</td>
<td>yes</td>
<td>1024</td>
<td></td>
<td>Max simultaneous connections.</td>
</tr>
<tr class="even">
<td>memcached_listen_host</td>
<td>yes</td>
<td>0.0.0.0</td>
<td></td>
<td>Memcached listen address.</td>
</tr>
<tr class="odd">
<td>memcached_listen_port</td>
<td>yes</td>
<td>11211</td>
<td></td>
<td>Memcached listen port.</td>
</tr>
<tr class="even">
<td>memcached_logfile</td>
<td>yes</td>
<td>/var/log/memcached.log</td>
<td></td>
<td>Log file location.</td>
</tr>
<tr class="odd">
<td>memcached_memory</td>
<td>yes</td>
<td></td>
<td>64</td>
<td>Max memory used for object storage.</td>
</tr>
</tbody>
</table>

Dependencies
------------

No additional role dependencies.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: hswong3i.memcached

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-memcached/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <a href="https://twitter.com/hswong3i" class="uri" class="uri">https://twitter.com/hswong3i</a>
    -   <a href="https://github.com/hswong3i" class="uri" class="uri">https://github.com/hswong3i</a>

