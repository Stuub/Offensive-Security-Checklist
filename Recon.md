---
tags #Recon #networkexploration #cybersecurity #osint
---

Recon is the first stage of a vulnerability analysis and [[exploitation]] routine in Offensive Security

This stage involves both Active and Passive recon.

### Active Recon

**NMAP**:

```
command: nmap -p 1-65535 -sV -sC <target IP>
---
description: network scanning tool. Discover open ports, identify services running on ports, gather information on the target system.
```

**Nessus:**

```
command: nessuscli scan --hosts <target IP> --template "Basic Network Scan"
---
description: vulnerability scanning tool. Provides detailed reports of results.
```

**Nikto:**

```
command: nikto -H <target-url>
---
description: automated vulnerability analysis tool for web apps, will crawl a domain and discover vulnerabilities and associated known exploits where possible.
```


**BurpSuite:**

```
command: burpsuite
---
description: Set up web proxy, intercept desired traffic and analyse for vulnerabilities
```

### Passive Recon

**Maltego**:

```
command: maltego <target domain>
---
description: OSINT tool to gather and visualise information on a target. Reveal entity relationships of domain names, IP addresses, social media profiles etc.
```

**theHarvester:**

```
command: theharvester -d <target domain> -b google
---
description: tool used for gathering email addresses, subdomains, and related info to target domain.
```

**[Shodan](https://www.shodan.io)**
```
Search Engine for IP devices. Search specific devices, services, vulnerabilities etc. Use case: Find devices, identify open ports, gather information on device.  
```

**Recon-ng:**

```
command: recon-ng
---
description: CLI-based framework, for information gathering about domains, IP's, email addresses etc.
```
 