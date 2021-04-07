<p align="center">
    <img src="https://static.magento.com/sites/all/themes/magento/logo.svg" width="300px" alt="Magento Commerce" />
</p>

#  Magento 1 Docker 

### Features

- Magento 1.9.*
- Apache
- PHP 7.2
- Xdebug 2.9.8
- MariaDB 10.4.13
- Elasticsearch 7.6
- Varnish 6.4
- Redis
- MailHog
- n98-magerun

### Requirements

**Linux:**

Install [Docker](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/) and [Docker-compose](https://docs.docker.com/compose/install/#install-compose).


### Before start
Note that for Elasticsearch you need at least 262144 memory. 

To check:
```
more /proc/sys/vm/max_map_count
```

The vm.max_map_count setting should be set permanently in `/etc/sysctl.conf`:
```
vm.max_map_count=262144
```
After set run:
```
sudo sysctl -p
```


### Panels

**Web server:** http://localhost/

**Local emails:** http://localhost:8025

### Features commands

| `bin/start` |
| `bin/stop`  |
| `bin/kill`  |
| `bin/shell` |
| `bin/magerun` | 
| `bin/gulp`    |
| `bin/xdebug`  |
|`bin/composer` | 
