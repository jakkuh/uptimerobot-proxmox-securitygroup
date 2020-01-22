# UptimeRobot Proxmox Firewall Security Group Ruleset
A security group ruleset for Proxmox firewalls to allow connections from UptimeRobot for server monitoring. This setup checks the destination port 8006 (the default port for the Proxmox Web UI), so if you have changed the port make sure you do so in the security group as well.

### Instructions
Copy the entire contents of `cluster.fw` in this repository into `/etc/pve/firewall/cluster.fw` on the Proxmox server you wish to use the Security Group on. Check the `Datacenter>Firewall>Security Group` tab to verify the Security Group was successfully added. Then add the Security Group to the firewall of the respective server you wish to allow UptimeRobot to monitor.

### Currently Allowed IPs (updated Jan 21, 2020):

```
69.162.124.224/28
63.143.42.240/28
216.245.221.80/28

104.131.107.63
122.248.234.23
128.199.195.156
138.197.150.151
139.59.173.249
146.185.143.14
159.203.30.41
159.89.8.111
165.227.83.148
178.62.52.237
18.221.56.27
188.226.183.141
216.144.250.150
34.233.66.117
46.101.250.135
46.137.190.132
52.60.129.180
54.64.67.106
54.67.10.127
54.79.28.129
54.94.142.218
```

Source: https://uptimerobot.com/locations
