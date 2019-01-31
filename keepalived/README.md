

## Environment Variables

* $IPS:
  * single-quoted, comma-delimited list of all hosts.
  * i.e.  '192.168.99.100', '192.168.99.101', '192.168.99.102'
* $VIP:
  * virtual ip.
  * i.e. 192.168.99.99


## Enable IPVS module

On all nodes which will participate in keepalived, we need the "ip_vs" kernel module, in order to permit serivces to bind to non-local interface addresses.

Set this up once for both the primary and secondary nodes, by running:

```
echo "modprobe ip_vs" >> /etc/rc.local
modprobe ip_vs
```

## References

https://geek-cookbook.funkypenguin.co.nz/ha-docker-swarm/keepalived/
https://github.com/osixia/docker-keepalived


