# 🛡 Task 8 - VPN and Privacy Protection

## 🔍 Objective:
Understand the role of VPNs in protecting privacy and secure communication by masking IP addresses and encrypting internet traffic.

---

## 🛠 Steps Performed:

1. ✅ Checked original public IP using [https://whatismyipaddress.com](https://whatismyipaddress.com)  
   - Result: IP - XXX.XXX.XXX.XXX (India - Real IP)

2. ✅ Installed and connected to a free VPN (Windscribe/ProtonVPN)

3. ✅ Verified new IP using:
   - Terminal command: curl ifconfig.me
   - Browser check: [https://whatismyipaddress.com](https://whatismyipaddress.com)  
   - Result: IP - XXX.XXX.XXX.XXX (USA - via Proxy/VPN)

4. ✅ Ran traffic capture:
   - Command: sudo tcpdump -i any port 80 or port 443
   - Observed encrypted traffic over the tun0 interface

---

## 🔐 Observations:

- *Before VPN*: Real IP - XXX.XXX.XXX.XXX (Location: India, ISP: Bharti Airtel)
- *After VPN*: IP changed to XXX.XXX.XXX.XXX (Location: USA, Detected as Proxy)
- *VPN Interface*: Activity detected on tun0 showing successful tunneling
- *tcpdump* confirms HTTPS (port 443) traffic encryption

---

## 🧠 Key Learnings:

- VPNs protect your online identity by masking IP addresses
- They use encryption and tunneling protocols for secure communication
- VPN traffic can be verified using packet analysis tools like tcpdump
- While VPNs improve privacy, they don't guarantee total anonymity

---

## 📸 Screenshots:

Stored in the screenshots/ folder:
- ip_before_vpn.png
- ip_after_vpn.png
- curl_ifconfig_output.png
- tcpdump_output.png

---

## ✅ Conclusion:

VPNs are powerful tools for enhancing privacy, especially on public or insecure networks. This task provided practical experience with VPNs, IP masking, and basic network traffic analysis.

---
