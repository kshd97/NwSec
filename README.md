1) Learned and drew a threat model diagram for a given network architecture
2) Prepared Wireshark for packet sniffing of a self-created environment consisting of a vulnerable system that is set up with a DHCP, DNS, Suricata, and a Term server using different Docker containers. This system was attacked using a Kali VM. Security was tightened by setting stricter rules for repeated sniffing in Suricata (Intrusion Detection).
3) Created a CTF challenge by introducing a vulnerability due to misconfiguration in an nginx webserver. The vulnerable system runs a telnet server that passes username and password in plaintext, this can be intercepted using Wireshark and used to attack the web server.
4) Used a Kali VM to explore HTTP-based Denial of Service (DoS) attacks on an Nginx web server on the target machine. Security can be enhanced using Intrusion Detection tools like Suricata and Nginx's own server settings.
5) Explored a Vulnerable Email server by setting up a vulnerable SMTP server using Docker. Used Wireshark from a Kali VM from the same network to spoof emails and users. Also ran attacks to obtain common passwords for users. Used SpamAssassin and Suricata for blocking spam attacks. Modified the POSTFix server to block emails with possible spam or phishing attacks.
6) Set up an insecure NFS+SSH server with password authentication using Docker. Then observed network sequences on Wireshark from Kali attack VM when a valid user mounts a file on the NFS shared location. Used Hydra on Kali to perform password-guessing attacks, and uploaded a malicious file to perform privilege escalation for the current users. This can be secured against using Suricata rules detection and deploying a Kerberos authentication server so that no usernames are exposed and password guessing is impossible
