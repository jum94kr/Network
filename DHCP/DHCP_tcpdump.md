## Discover

<pre>
tcpdump: listening on svpn0, link-type EN10MB (Ethernet), capture size 65535 bytes
08:59:57.698477 IP (tos 0x0, ttl 128, id 25934, offset 0, flags [none], proto UDP (17), length 328)
    0.0.0.0.68 > 255.255.255.255.67: [udp sum ok] BOOTP/DHCP, Request from ca:fe:03:91:xx:3f, length 300, xid 0x383394cd, Flags [none] (0x0000)
          Client-Ethernet-Address ca:fe:03:91:xx:3f
          Vendor-rfc1048 Extensions
            Magic Cookie 0x63825363
            DHCP-Message Option 53, length 1: Discover
            Client-ID Option 61, length 7: ether ca:fe:03:91:xx:3f
            Hostname Option 12, length 15: "DESKTOP"
            Vendor-Class Option 60, length 8: "MSFT 5.0"
            Parameter-Request Option 55, length 14: 
              Subnet-Mask, Default-Gateway, Domain-Name-Server, Domain-Name
              Router-Discovery, Static-Route, Vendor-Option, Netbios-Name-Server
              Netbios-Node, Netbios-Scope, Option 119, Classless-Static-Route
              Classless-Static-Route-Microsoft, Option 252
            END Option 255, length 0
            PAD Option 0, length 0, occurs 4
</pre>

## Offer

<pre>
08:59:58.706718 IP (tos 0x10, ttl 128, id 0, offset 0, flags [none], proto UDP (17), length 328)
    192.168.10.1.67 > 192.168.10.5.68: [udp sum ok] BOOTP/DHCP, Reply, length 300, xid 0x383394cd, Flags [none] (0x0000)
          Your-IP 192.168.10.5
          Client-Ethernet-Address ca:fe:03:91:xx:3f
          Vendor-rfc1048 Extensions
            Magic Cookie 0x63825363
            DHCP-Message Option 53, length 1: Offer
            Server-ID Option 54, length 4: 192.168.10.1
            Lease-Time Option 51, length 4: 86400
            Subnet-Mask Option 1, length 4: 255.255.255.0
            Default-Gateway Option 3, length 4: 192.168.10.1
            Domain-Name-Server Option 6, length 4: 8.8.8.8
            END Option 255, length 0
            PAD Option 0, length 0, occurs 26
</pre>

## Request

<pre>
08:59:58.713662 IP (tos 0x0, ttl 128, id 25935, offset 0, flags [none], proto UDP (17), length 356)
    0.0.0.0.68 > 255.255.255.255.67: [udp sum ok] BOOTP/DHCP, Request from ca:fe:03:91:xx:3f, length 328, xid 0x383394cd, Flags [none] (0x0000)
          Client-Ethernet-Address ca:fe:03:91:xx:3f
          Vendor-rfc1048 Extensions
            Magic Cookie 0x63825363
            DHCP-Message Option 53, length 1: Request
            Client-ID Option 61, length 7: ether ca:fe:03:91:xx:3f
            Requested-IP Option 50, length 4: 192.168.10.5
            Server-ID Option 54, length 4: 192.168.10.1
            Hostname Option 12, length 15: "DESKTOP"
            FQDN Option 81, length 18: "DESKTOP"
            Vendor-Class Option 60, length 8: "MSFT 5.0"
            Parameter-Request Option 55, length 14: 
              Subnet-Mask, Default-Gateway, Domain-Name-Server, Domain-Name
              Router-Discovery, Static-Route, Vendor-Option, Netbios-Name-Server
              Netbios-Node, Netbios-Scope, Option 119, Classless-Static-Route
              Classless-Static-Route-Microsoft, Option 252
            END Option 255, length 0
</pre>

## ACK

 <pre>   
08:59:58.716320 IP (tos 0x10, ttl 128, id 0, offset 0, flags [none], proto UDP (17), length 328)
    192.168.10.1.67 > 192.168.10.5.68: [udp sum ok] BOOTP/DHCP, Reply, length 300, xid 0x383394cd, Flags [none] (0x0000)
          Your-IP 192.168.10.5
          Client-Ethernet-Address ca:fe:03:91:xx:3f
          Vendor-rfc1048 Extensions
            Magic Cookie 0x63825363
            DHCP-Message Option 53, length 1: ACK
            Server-ID Option 54, length 4: 192.168.10.1
            Lease-Time Option 51, length 4: 86400
            Subnet-Mask Option 1, length 4: 255.255.255.0
            Default-Gateway Option 3, length 4: 192.168.10.1
            Domain-Name-Server Option 6, length 4: 8.8.8.8
            END Option 255, length 0
            PAD Option 0, length 0, occurs 26
</pre>

## Release

<pre>
09:00:16.089488 IP (tos 0x0, ttl 128, id 40499, offset 0, flags [none], proto UDP (17), length 328)
    192.168.10.5.68 > 192.168.10.1.67: [udp sum ok] BOOTP/DHCP, Request from ca:fe:03:91:xx:3f, length 300, xid 0x383398b5, Flags [none] (0x0000)
          Client-IP 192.168.10.5
          Client-Ethernet-Address ca:fe:03:91:xx:3f
          Vendor-rfc1048 Extensions
            Magic Cookie 0x63825363
            DHCP-Message Option 53, length 1: Release
            Server-ID Option 54, length 4: 192.168.10.1
            Client-ID Option 61, length 7: ether ca:fe:03:91:xx:3f
            END Option 255, length 0
            PAD Option 0, length 0, occurs 41
</pre>
