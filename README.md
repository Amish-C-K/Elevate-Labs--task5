# 🛡️ Task 5: Capture and Analyze Network Traffic Using Wireshark

## 🎯 Objective
Capture live network packets using Wireshark and analyze the captured traffic to identify basic network protocols and understand how devices communicate over a network.

---

## 🧰 Tools Used
- **Wireshark** (Free and Open Source)
- System browser and terminal (to generate traffic)

---

## 🧪 Steps Performed

1. ✅ Installed and launched **Wireshark**.
2. ✅ Started capture on the **active network interface (Wi-Fi)**.
3. ✅ Browsed multiple websites and used `ping` to generate traffic:
   ```bash
   ping google.com
   ```
4. ✅ Captured traffic for **approximately 1 minute**.
5. ✅ Stopped and saved the capture as `network-traffic-task5.pcapng`.
6. ✅ Analyzed protocols using filters and **Statistics → Protocol Hierarchy**.

---

## 🔍 Identified Protocols

| Protocol   | Description                                                                 |
|------------|-----------------------------------------------------------------------------|
| `ICMP`     | Used for diagnostic functions like `ping` and error reporting.             |
| `ICMPv6`   | IPv6 version of ICMP, used for neighbor discovery and error reporting.     |
| `TCP`      | Reliable transmission protocol used for most internet communications.      |
| `DNS`      | Resolves domain names to IP addresses.                                     |
| `ARP`      | Maps IP addresses to MAC addresses on the local network.                   |
| `TLSv1.3`  | Encrypts data for secure communications (used in HTTPS).                   |
| `HTTP`     | Transmits web content without encryption (used on port 80).                |
| `OCSP`     | Checks the status of digital certificates (used by browsers).             |
| `QUIC`     | Modern secure transport protocol by Google, used by services like YouTube. |

---

## 🧾 Sample Packet Insights

### 🔹 ICMP
- **Type**: Echo (Ping) Request  
- **Destination**: 8.8.8.8 (Google DNS)

### 🔹 DNS
- **Query**: A record for `example.com`  
- **Port**: 53 (UDP)

### 🔹 TCP
- **Flags**: SYN, ACK  
- **Purpose**: Connection setup to `openai.com:443`

### 🔹 TLS v1.3
- **Details**: Client Hello  
- **Purpose**: Encrypted handshake for HTTPS session

### 🔹 HTTP
- **Request**: `GET / HTTP/1.1`  
- **Port**: 80  
- **Host**: `example.com`

---

## 📁 Deliverables

- 📦 Packet Capture File: `network-traffic-task5.pcapng`
- 📝 This report in `README.md` format

---

## ✅ Outcome

This hands-on exercise helped me gain practical experience with Wireshark, understand how common internet protocols operate, and visualize real-time network activity and communication flow between systems.

---

> _Created as part of a cybersecurity learning module._
