Fourth task of the cyber security internship

Firewall Rules Configuration - Kali Linux using UFW

Objective
To configure, test, and document basic firewall rules using UFW (Uncomplicated Firewall) on Kali Linux, including blocking and allowing traffic on specific ports.

Tasks Performed

1. Installed and enabled UFW to manage firewall rules.
2. Listed current firewall rules to check the default state.
3. Blocked inbound traffic on port 23 (Telnet) using:
   sudo ufw deny 23
4. Tested the rule using Telnet/Netcat to ensure port 23 was blocked.
5. Allowed SSH traffic on port 22 to ensure remote access remained active:
   sudo ufw allow 22
6. Removed the Telnet block rule to restore the original configuration:
   sudo ufw delete deny 23
7. Took screenshots of firewall status before, during, and after applying the rules.

Testing

- Used `telnet localhost 23` and `nc -v localhost 23` to confirm the port was successfully blocked.
- Verified SSH (port 22) was still accessible.

Summary

UFW was used to demonstrate basic firewall rule management on Kali Linux. The firewall filtered traffic based on port numbers and direction, allowing secure traffic (SSH) while blocking insecure or unused ports (Telnet).

Files
- Terminal screenshots showing:
  - Firewall Rules.png
  - Firewall Default.png
  - Firewall Configuration.pdf
