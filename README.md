Redis-role
=========

This role installs redis server.

Variables
======
All variables that should be configured stored in redis_conf dictionary.
There is not much to configure with redis.
~~~
redis_conf:
  host: '127.0.0.1'
  password: 'change_me'
  datadir: '/var/lib/redis'
~~~

Zabbix support
======
To enable zabbix support you should setup zabbix_url variable

Also your inventory should contain zabbix variables for host.
Example:
~~~
zabbix_url: 'http://zabbix.example.com'   # host url for zabbix server
zabbix_user: 'Admin'                      # username
zabbix_pass: 'change_me'                  # password
zabbix_dir: '/etc/zabbix/zabbix_agentd.d' # directory that contains userparameters
~~~
