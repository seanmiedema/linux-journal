sean@sean-XPS-13-9365:~$ uname -a
Linux sean-XPS-13-9365 6.17.0-14-generic #14~24.04.1-Ubuntu SMP PREEMPT_DYNAMIC Thu Jan 15 15:52:10 UTC 2 x86_64 x86_64 x86_64 GNU/Linux
sean@sean-XPS-13-9365:~$ df -h
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           782M  2.1M  780M   1% /run
efivarfs        374K  138K  232K  38% /sys/firmware/efi/efivars
/dev/nvme0n1p2  468G   37G  408G   9% /
tmpfs           3.9G     0  3.9G   0% /dev/shm
tmpfs           5.0M  8.0K  5.0M   1% /run/lock
/dev/nvme0n1p1  511M  6.2M  505M   2% /boot/efi
tmpfs           782M  256K  781M   1% /run/user/1000
sean@sean-XPS-13-9365:~$ free -m
               total        used        free      shared  buff/cache   available
Mem:            7810        3194        1024         592        4504        4616
Swap:           2047           0        2047
sean@sean-XPS-13-9365:~$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host noprefixroute 
       valid_lft forever preferred_lft forever
2: wlp60s0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue state UP group default qlen 1000
    link/ether f8:63:3f:4a:c6:a3 brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.212/24 brd 192.168.1.255 scope global dynamic noprefixroute wlp60s0
       valid_lft 84229sec preferred_lft 84229sec
    inet6 fda0:7c95:dcc5:4be4:ace9:e514:c857:feec/64 scope global temporary dynamic 
       valid_lft 1741sec preferred_lft 1741sec
    inet6 fda0:7c95:dcc5:4be4:c29c:4c5b:48b9:3176/64 scope global dynamic mngtmpaddr noprefixroute 
       valid_lft 1741sec preferred_lft 1741sec
    inet6 fe80::9d02:8e75:6c2d:6680/64 scope link noprefixroute 
       valid_lft forever preferred_lft forever
3: tailscale0: <POINTOPOINT,MULTICAST,NOARP,UP,LOWER_UP> mtu 1280 qdisc fq_codel state UNKNOWN group default qlen 500
    link/none 
    inet 100.126.90.36/32 scope global tailscale0
       valid_lft forever preferred_lft forever
    inet6 fd7a:115c:a1e0::7b33:5a24/128 scope global 
       valid_lft forever preferred_lft forever
    inet6 fe80::3f90:961:b2fe:11a5/64 scope link stable-privacy 
       valid_lft forever preferred_lft forever
