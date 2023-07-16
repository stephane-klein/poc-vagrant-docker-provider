# POC Vagrant with Docker provider

This POC use https://github.com/tknerr/vagrant-docker-baseimages

```sh
$ vagrant up
$ vagrant ssh
vagrant@546123df733a:~$ sudo su
root@546123df733a:/home/vagrant# apt install htop
root@546123df733a:/home/vagrant# htop
    0[              0.0%]    4[              0.0%]     8[              0.0%]   12[              0.0%]
    1[              0.0%]    5[              0.0%]     9[              0.0%]   13[              0.0%]
    2[              0.0%]    6[              0.0%]    10[              0.0%]   14[              0.0%]
    3[              0.0%]    7[              0.0%]    11[              0.0%]   15[              0.0%]
  Mem[||||||||||||||||||||||||||||||||8.50G/30.1G]   Tasks: 10, 0 thr; 1 running
  Swp[|                                512K/8.00G]   Load average: 0.55 0.86 1.62
                                                     Uptime: 2 days, 19:53:57

    PID USER      PRI  NI  VIRT   RES   SHR S CPU%-MEM%   TIME+  Command
      1 root       20   0  2888  1536  1536 S  0.0  0.0  0:00.00 /bin/sh -c /usr/sbin/sshd -D     -o UseDN
      7 root       20   0 15424  9088  7552 S  0.0  0.0  0:00.00 sshd: /usr/sbin/sshd -D -o UseDNS=no -o U
    717 root       20   0 15732  9600  7936 S  0.0  0.0  0:00.00 sshd: vagrant [priv]
    719 vagrant    20   0 16332  7332  5248 S  0.0  0.0  0:00.01 sshd: vagrant@pts/0
    720 vagrant    20   0  4624  3584  3072 S  0.0  0.0  0:00.00 -bash
    724 root       20   0  8092  4992  4352 S  0.0  0.0  0:00.00 sudo su
    725 root       20   0  8092  1980  1408 S  0.0  0.0  0:00.00 sudo su
    726 root       20   0  7032  4480  3968 S  0.0  0.0  0:00.00 su
    727 root       20   0  4624  3712  3200 S  0.0  0.0  0:00.00 bash
    734 root       20   0  5260  3968  3072 R  0.0  0.0  0:00.00 htop
```

```sh
$ vagrand destroy -f
```
