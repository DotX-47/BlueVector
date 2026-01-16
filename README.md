# 🔵 BlueVector

BlueVector is a modular Python-based network analysis and security toolkit developed by **DotX**.  
It provides a menu-driven interface for performing common networking, scanning, and inspection tasks in a controlled and authorized environment.

---

## 📸 Tool Output Preview

![BlueVector Output](BlueVectoor/Image1.png)


## 📌 What is BlueVector?

BlueVector combines multiple network utilities into a single command-line tool.  
It is designed to help understand:
- How networks respond to probes
- How services expose ports and banners
- How systems can be inspected from a defensive security perspective

BlueVector is suitable for:
- Internal company testing
- Research and learning
- Authorized security assessments

> ⚠️ Use only on systems you own or have explicit permission to test.

---

## 🧰 Included Modules (Detailed Explanation)

### 1️⃣ Get IP (DNS Resolver)
Resolves a domain name into its corresponding IP address using DNS.

**Example:**
- Input: `github.com`
- Output: `140.82.113.3`

**Purpose:** Understand DNS resolution  
**OS Support:** Windows & Linux

---

### 2️⃣ Ping Sweep
Pings a range of IP addresses to determine which hosts are online.

**Purpose:**
- Network discovery
- Identifying active devices

**OS Support:** Windows & Linux

---

### 3️⃣ Traceroute
Displays the network path packets take to reach a target host.

**Windows:** Uses `pathping`  
**Linux:** Requires `traceroute` (code adjustment recommended)

**Purpose:** Routing and latency analysis

---

### 4️⃣ TCP Sweep
Checks a specific TCP port across multiple IP addresses to find active services.

**Purpose:**
- Identify systems running a known service
- Asset discovery

**OS Support:** Windows & Linux

---

### 5️⃣ Port Scanner
Performs a multi-threaded scan of TCP ports on a single target.

**Purpose:**
- Identify open ports
- Understand service exposure

**OS Support:** Windows & Linux

---

### 6️⃣ Banner Grabber
Connects to a service and attempts to read its banner.

**Purpose:**
- Service identification
- Version awareness

**OS Support:** Windows & Linux

---

### 7️⃣ Hyperlink Extractor
Downloads a webpage and extracts all hyperlinks.

**Purpose:**
- Website structure analysis
- OSINT-style inspection

**OS Support:** Windows & Linux

---

### 8️⃣ WMI Module (Windows Only)
Uses Windows Management Instrumentation (WMI) to query remote Windows systems.

**Capabilities:**
- OS information
- Running services
- Processes
- Users and groups

**OS Support:** Windows only

---

<p align="center">
  <img src="BlueVector/Image2.png" width="800">
</p>


## 🖥️ System Requirements

- Python **3.7 or higher**
- Windows or Linux
- Network connectivity

---

## 📦 Installation & Download

### 🔹 Method 1: GitHub Clone (Recommended)
```bash
git clone https://github.com/DotX-47/BlueVector.git
cd BlueVector
```



Extract the ZIP and navigate into the folder.

---

## 📚 Dependencies

Install required Python libraries:

```bash
pip install -r requirements.txt
```
Or

```bash
pip install beautifulsoup4 wmi
```

> Linux users can skip `wmi`.

---

## 🚀 How to Use

### Windows
```bat
python BlueVector.py
```

### Linux
```bash
python3 BlueVector.py
```

After launching, choose a module from the menu by entering its number.

---

## 🔐 Legal & Ethical Use

BlueVector must be used only on:
- Systems you own
- Systems you manage
- Systems you have written permission to test

Unauthorized scanning or access is illegal.

---

## 👤 Author

**DotX-47**  
GitHub: https://github.com/DotX-47

---

## 📄 Disclaimer

This software is provided "as is" without warranty of any kind.  
The author is not responsible for misuse or damage caused by this tool.
