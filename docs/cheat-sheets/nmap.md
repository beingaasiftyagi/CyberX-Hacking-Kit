# Nmap Cheat Sheet 📊

> **⚠️ Legal Note**: Only use on networks you own or have permission to scan

## 🔍 Basic Scans
```bash
nmap 192.168.1.1             # Basic TCP port scan
nmap -sP 192.168.1.0/24      # Ping sweep (discover live hosts)
nmap -p 22,80,443 <target>   # Scan specific ports
nmap -F <target>             # Fast scan (100 common ports)
```

## 🛠️ Advanced Scanning
```bash
nmap -A <target>             # Aggressive scan (OS, version, script)
nmap -sV -O <target>         # Service and OS detection
nmap -T4 <target>            # Faster scan (timing template 4)
nmap -Pn <target>            # Skip host discovery (treat all as up)
```

## 🕵️ Stealth Techniques
```bash
nmap -sS <target>            # SYN scan (half-open)
nmap -sT <target>            # TCP connect scan
nmap -sU <target>            # UDP scan (slow but important)
nmap -f <target>             # Fragment packets (evade detection)
```

## 📝 Output Formats
```bash
nmap -oN scan.txt <target>   # Normal output
nmap -oX scan.xml <target>   # XML output
nmap -oG scan.gnmap <target> # Grepable output
nmap -oA scan <target>       # All formats (normal, XML, grepable)
```

## 🎯 Common Ports Cheat Sheet
| Port | Service       | Common Vulnerabilities |
|------|---------------|------------------------|
| 21   | FTP           | Anonymous login        |
| 22   | SSH           | Weak passwords         |
| 80   | HTTP          | Web vulnerabilities    |
| 443  | HTTPS         | SSL/TLS issues         |
| 3306 | MySQL         | Default credentials    |

## 🧰 Useful NSE Scripts
```bash
nmap --script=http-title <target>       # Get webpage titles
nmap --script=vuln <target>             # Vulnerability scanning
nmap --script=ssl-enum-ciphers <target> # Check SSL/TLS ciphers
```

## 📚 Resources
- [Official Nmap Documentation](https://nmap.org/docs.html)
- [Nmap Network Scanning Book](https://nmap.org/book/)
- [Nmap Scripting Engine Guide](https://nmap.org/book/nse.html)

> Remember to always get proper authorization before scanning!
```

4. **Commit your changes**:
   - Scroll down to the commit section
   - Add a commit message like "Added comprehensive Nmap cheat sheet"
   - Choose "Commit directly to the main branch"
   - Click "Commit changes"

## What Makes This Cheat Sheet Effective:

1. **Clear Organization**:
   - Section headers with emojis for visual scanning
   - Logical flow from basic to advanced commands

2. **Practical Content**:
   - Most commonly used Nmap commands
   - Ready-to-copy code blocks
   - Common ports reference table

3. **Legal Protection**:
   - Prominent disclaimer at top
   - Warning in the commit message

4. **Additional Resources**:
   - Links to official documentation
   - Reference materials. 
