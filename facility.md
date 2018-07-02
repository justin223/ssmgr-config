## SELinux
```bash
semanage port -a -t openvpn_port_t -p tcp 8387-8388
semanage port -a -t openvpn_port_t -p udp 8387-8388
```

## FirewallD
```bash
firewall-cmd --add-port=8387-8388/tcp --permanent
firewall-cmd --reload
```
