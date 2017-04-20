# linux-item-catalog
A linux server that host an Item Catalog application.

## IP & connections
- IP `52.206.20.209`
- Enabled ports
    - 2200 ssh
    - 80 http
    - 123 ntp

## TODO
- [x] New server instance on _Amazon Lightsail_.
- [x] Change SSH port from 22 to 2200.
- [x] Configure UFW to only allow connections for SSH port2200, HTTP port 80 and NTP port 123.
- [x] Create user __grader__.
- [x] Allow __grader__ to perfoem `sudo`.
- [x] Create ssh key pair for __grader__.
- [x] Configure local timezone to UTC.
- [ ] Install and configure Apache & Python mod_wsgi.
- [ ] Install and configure PostgreSQL.
- [ ] Create database user name __catalog__ with limited permissions.
- [ ] Install git.
- [ ] Clone and setup [Item Catalog Application](https://github.com/oscarchang1226/udacity-catalog).

## Sources
- [Linux Configuration](https://github.com/jrleszcz/linux-server-setup/blob/master/how-to/configure-firewall-and-change-ssh-port.md)
- [Ubuntu Updating Packages](https://www.digitalocean.com/community/questions/updating-ubuntu-14-04-security-updates)
