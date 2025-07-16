## Network Tools & Packet Capture

### 🛠 Tools Practiced:
- `netstat -tuln` → Checked listening TCP/UDP ports
- `ss -tulwn` → Faster replacement for netstat
- `whois` → Found domain registration info
- `dig`, `nslookup` → Queried DNS records (A, MX, NS)
- `ping`, `traceroute` → Tested reachability and route
- `tcpdump` → Captured 20 packets and saved as `.pcap`

### 💡 Key Learnings:
- `Send-Q` shows queued data still not sent
- `Peer Address` helps track remote connections
- `tcpdump -w` captures continuously until Ctrl+C
- `traceroute` showed each hop from VM to domain
- Understood basic real-time traffic flow using tcpdump

### ⚠️ Notes:
- Wireshark not used (optional for now)
- Pushed blank file first by mistake — fixed ✅
