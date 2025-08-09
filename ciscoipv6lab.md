hello, this is a paper trail of my learning of IPv6 using mostly cisco hardware.

Resource:
1. Cisco 1921 Router with 2 gigabitethernet ports 0/0 and 0/1
2. Cisco ASA 5520 Firewall
3. Cisco 2960
4. Uspeed wifi router (300mbps max)
5. Linksys AC1200
6. my lab computer (putty and this git)


day 1: Preparing the router
- I started with getting into the router.
    - I turned off ip domain lookup
          Router (config)#no ip domain lookup
      this ensures that any commands it does not recognize, does not get translated, since it is a hassle.
    - I enabled ipv6 via
          Router(config)# ipv6 unicast-routing
      enables the forwarding of IPv6 packets. Without this command, the router won't participate in IPv6 routing, even if IPv6 addresses are configured on its interfaces
that is the end of day 1.
