# linux-item-catalog
A linux server that host an Item Catalog application.

## IP & connections
- IP `52.206.20.209`
- Enabled ports
    - 2200 ssh
    - 80 http
    - 123 ntp

## URL
[http://52.206.20.209/](http://52.206.20.209/)

## SSH Key for `grader`
Located in the path `/home/grader/.ssh`

## Installed Software
- postgresql python-psycopg2
- python-sqlalchemy
- python-pip
    - werkzeug==0.8.3
    - flask==0.9
    - Flask-Login==0.1.3
    - oauth2client
    - requests
    - httplib2
    - bleach

## TODO
- [x] New server instance on _Amazon Lightsail_.
- [x] Change SSH port from 22 to 2200.
- [x] Configure UFW to only allow connections for SSH port2200, HTTP port 80 and NTP port 123.
- [x] Create user __grader__.
- [x] Allow __grader__ to perfoem `sudo`.
- [x] Create ssh key pair for __grader__.
- [x] Configure local timezone to UTC.
- [x] Install and configure Apache & Python mod_wsgi.
- [x] Install and configure PostgreSQL.
- [x] Create database user name __catalog__ with limited permissions.
- [x] Install git.
- [x] Clone and setup [Item Catalog Application](https://github.com/oscarchang1226/udacity-catalog).

## Notes
- [Google OAuth for public IP not available.](http://stackoverflow.com/questions/14238665/can-a-public-ip-address-be-used-as-google-oauth-redirect-uri)

## Sources
- [Linux Configuration](https://github.com/jrleszcz/linux-server-setup/blob/master/how-to/configure-firewall-and-change-ssh-port.md)
- [Ubuntu Updating Packages](https://www.digitalocean.com/community/questions/updating-ubuntu-14-04-security-updates)
- [SQLAlchemy Quickstart with PostgreSQL](https://suhas.org/sqlalchemy-tutorial/)
- [Flask Setup](http://flask.pocoo.org/docs/0.12/deploying/mod_wsgi/)
