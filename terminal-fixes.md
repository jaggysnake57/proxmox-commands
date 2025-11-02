## fix corrupt console

```
# 1. Remove stale dtach socket for CT 202
rm -f /var/run/dtach/vzctlconsole202

# 2. Restart Proxmox daemons that handle console and web access
systemctl restart pvedaemon pveproxy pvestatd

# 3. (Optional) Restart the container if needed
pct restart 202
```
