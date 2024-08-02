# Deathnote-vulhub-Report
This repository contains a detailed report on the penetration testing of the Deathnote VulnHub machine. The objective was to gain root access through various exploitation techniques.

This repository features a comprehensive report on the penetration testing of the Deathnote VulnHub machine, aimed at gaining root access through various exploitation techniques. The project details the environment setup using Oracle VirtualBox, with the target IP configured as 10.10.0.2, and lists tools employed, including Nmap, Gobuster, WPScan, and Hydra.

Key vulnerabilities identified include insecure configurations in OpenSSH and Apache HTTP Server, an outdated WordPress version, and weak password practices. The report outlines a systematic approach taken to exploit these vulnerabilities, starting with port scanning using Nmap to identify open ports and services. Directory enumeration with Gobuster revealed critical paths, including a WordPress directory and hints in the robots.txt file.

Subsequent steps included analyzing an image file for hidden content, conducting WordPress enumeration to discover user accounts, and running WPScan to identify vulnerabilities. A brute force attack using Hydra successfully uncovered SSH credentials, allowing access as user "l."

Privilege escalation was achieved by locating the "kira" user, exploiting insecure file permissions, and decoding a password from a suspicious file. Ultimately, the report emphasizes the lessons learned regarding the importance of thorough enumeration, keeping software updated, implementing robust password policies, and securing file permissions.
