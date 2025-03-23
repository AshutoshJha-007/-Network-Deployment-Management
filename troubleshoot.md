# Troubleshooting Guide for ISP Network

## Common Network Issues & Solutions

### 1. **No Internet Connectivity**
- **Check WAN Connection:** Ensure the main router has an active internet connection.
- **Verify IP Configuration:** Run `ifconfig` (Linux) or `ipconfig` (Windows) to check IP settings.
- **Restart Network Devices:** Power cycle OLT, ONU, router, and switches.

### 2. **Slow Network Performance**
- **Check Bandwidth Usage:** Use `iftop` or `nload` to monitor real-time traffic.
- **Optimize QoS Settings:** Prioritize critical traffic on the router.
- **Inspect Cables & Connections:** Replace faulty Ethernet or fiber optic cables.

### 3. **Devices Not Getting IP Addresses**
- **Check DHCP Server Logs:** Run `journalctl -u isc-dhcp-server --no-pager`.
- **Verify Subnet Configuration:** Ensure DHCP pool matches network subnet.
- **Restart DHCP Service:** `sudo systemctl restart isc-dhcp-server`.

### 4. **DNS Resolution Issues**
- **Test Name Resolution:** Run `nslookup google.com` or `dig google.com`.
- **Restart DNS Server:** `sudo systemctl restart bind9`.
- **Flush DNS Cache:** `systemd-resolve --flush-caches` (Linux), `ipconfig /flushdns` (Windows).

### 5. **Packet Loss & High Latency**
- **Run Ping Tests:** `ping -c 10 8.8.8.8`.
- **Trace Network Path:** `traceroute 8.8.8.8` (Linux), `tracert 8.8.8.8` (Windows).
- **Check Switch Port Errors:** `show interfaces status` on managed switches.

### 6. **Fiber Optic Issues**
- **Check Light Levels:** Use an Optical Power Meter to measure signal strength.
- **Inspect Physical Damage:** Replace or re-splice broken fiber cables.

---
For advanced troubleshooting, refer to vendor-specific documentation and logs.
