# ✅ Day 04: Linux Recon & Nmap Scanning

## 🧠 What I Learned:

### 🔹 Linux Basics (Continued)
- Deep dive into `ip a`, `sudo`, `permissions`, and system structure
- Understood system loopback (127.0.0.1) vs active network IPs

### 🔹 Nmap Scanning Techniques
- ✅ `nmap localhost` – scanned open ports on the VM
- ✅ `nmap -sV 192.168.x.x` – service version detection
- ✅ `nmap -A -Pn` – aggressive scan with OS, service, traceroute
- ✅ `nmap -sS -Pn` – stealth SYN scan (low footprint)

### 🔹 Issues Faced
- OS scan returned "Too many fingerprints" on VM
- RTTvar too high on some scans → adjusted timing with `-T3`
- Realized scanning the same VM from within itself gives noisy results

### 🛠️ Fixes & Workarounds
- Used `-Pn` to skip ping checks on firewalled devices
- Scanned router & host machine to get better results
- Learned difference between scanning loopback, VM, and external targets

---

## 🔚 Key Takeaways:
- Stealthy scans help bypass firewalls
- OS detection is not always reliable inside VMs
- Use `ipconfig` (host) and `ip a` (VM) to get correct targets
