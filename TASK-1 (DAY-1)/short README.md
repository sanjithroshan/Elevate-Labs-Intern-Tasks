TASK 1 (DAY 1)
1.I opened my terminal and ran the command:
     i) nmap -sS 192.168.1.3/24
    ii)This told Nmap to do a stealth (SYN) scan on all devices from 192.168.1.1 to 192.168.1.255 on my local network.

2.Nmap sent scan packets to the 1,000 most common TCP ports on every device it found in that network range.

3.For each device that was online, Nmap checked which ports were open and what services were running on them.

4.According to the scan results:

    i)At 192.168.1.1, ports 53 (DNS), 80 (HTTP), 443 (HTTPS), and 5555 (Freeciv/ADB) were open.
   ii)Two other devices, 192.168.1.3 and 192.168.1.9, were online but had all common ports closed.

5.I summarized the risks of these open ports:

53/tcp (DNS): Can be abused for DDoS, amplification, or spoofing attacks.

80/tcp (HTTP): Vulnerable to data sniffing, man-in-the-middle attacks, XSS, SQL injection, and other web exploits.

443/tcp (HTTPS): Risks include misconfiguration, outdated SSL/TLS, app vulnerabilities, and certificate spoofing.

5555/tcp (Freeciv/ADB): Can allow remote device takeover, malware infections, full system compromise (if ADB), and Denial of Service attacks.