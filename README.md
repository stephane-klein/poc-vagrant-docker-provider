# POC Vagrant with Docker provider

This POC use https://github.com/tknerr/vagrant-docker-baseimages

```sh
$ vagrant up
$ vagrant ssh
vagrant@546123df733a:~$ sudo su
root@10f479a510b5:/home/vagrant# systemctl status
System has not been booted with systemd as init system (PID 1). Can't operate.
Failed to connect to bus: Host is down
```

```sh
$ vagrand destroy -f
```
