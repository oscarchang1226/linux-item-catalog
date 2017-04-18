#Linux Notes

## User Managament
- User info stored in `/etc/passwd`

### Adding User
`sudo adduser newuser`

### Login as User
`ssh newuser@ip_address -p portnum`

### Grant `sudo` to new User
1. List sudoers with `/etc/sudoers.d`
2. Copy file of a sudoer
3. In the copied file change the username to new user

### Key Based Authentication
1. generate key using `ssh-keygen`.
    - Default file name:`.../Users/user/.ssh/keyname`
2. install key into remote server
    - In remote server create a file `./.ssh/authorized_keys` in the home directory.
    - Copy generated key in local machine from `keyname.pub`.
    - paste into `authorized_keys`
    - chmod `authorized_keys` to 700
3. Test login with
`ssh newuser@ip_address -p portnum -i key_file_path`

### Enforcing Key Based Authentication
1. configure passwordauthentication to no in `/etc/ssh/sshd_config` file.
2. restart server with `sudo service ssh restart`
