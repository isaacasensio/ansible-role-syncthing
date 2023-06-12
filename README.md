Syncthing
=========

Syncthing replaces proprietary sync and cloud services with something open, trustworthy and decentralized. Your data is your data alone and you deserve to choose where it is stored, if it is shared with some third party and how it's transmitted over the Internet.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
syncthing_image: "lscr.io/linuxserver/syncthing:latest"
```
The version of the docker image to run as a container.

```
syncthing_host_config_path: /etc/syncthing
```
Host path which stores syncthing configuration.

```
syncthing_host_data_path: /var/lib/syncthing
```
Host path which stores syncthing data.

```
syncthing_container_user: syncthing
```
user running the container 

```
syncthing_timezone: "Europe/Madrid"
```
timezone for cron job

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - iasensio.syncthing

License
-------

MIT

