## Understandng the output of ip addr.
-- priyanshu_vishwakarma@Priyanshu-vishw:~$ ip addr
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet 10.255.255.254/32 brd 10.255.255.254 scope global lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host 
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq state UP group default qlen 1000
    link/ether 00:15:5d:b4:a9:86 brd ff:ff:ff:ff:ff:ff
    inet 172.29.107.232/20 brd 172.29.111.255 scope global eth0
       valid_lft forever preferred_lft forever
    inet6 fe80::215:5dff:feb4:a986/64 scope link 
       valid_lft forever preferred_lft forever
- output :-- 1: lo = loopback ( Loopback is a virtual network through which our computer/system can communicate with itself. )
                - 127.0.0.1 = is local host
                - UP = means interface is active.
                - mtu 65536 = means Maximun Packet Size
   - 2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> = This is actual network card
   - 172.29.107.232 = it my private ip address (always shows or use on local not on internet )
   - 172.29.107.232/20 = /20 shows cidr notation (shows the network size)
   - state up = means network is working
   - lower up = means physical connection is also active
   - link/ether 00:15:5d:b4:a9:86 = MAC address
   - brd 172.29.111.255 = broadcast address
   - inet6 fe80::215:5dff:feb4:a986/64 = ipv6 address
- https://chatgpt.com/share/69883990-02a0-8008-a2a3-4a2f200d8ec6
- 
