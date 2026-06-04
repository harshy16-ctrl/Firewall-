# Cyber Security Internship - Task 4: Setup and Use a Firewall on Windows/Linux

**Author:** Harsh Yadav

## Objective
Configure and test basic firewall rules to allow or block network traffic.

## Tools Used
- Windows Firewall / UFW (Linux)
- Command Prompt / Terminal

## Steps Performed

### Linux (UFW)
1. Checked UFW status:
   ```bash
   sudo ufw status verbose
   ```
2. Blocked Telnet port 23:
   ```bash
   sudo ufw deny 23
   ```
3. Allowed SSH port 22:
   ```bash
   sudo ufw allow 22
   ```
4. Verified rules:
   ```bash
   sudo ufw status numbered
   ```
5. Removed test rule:
   ```bash
   sudo ufw delete deny 23
   ```

### Windows Firewall
1. Opened Windows Defender Firewall with Advanced Security.
2. Created a new Inbound Rule.
3. Selected Port → TCP → Specific Port 23.
4. Chose Block the Connection.
5. Applied rule and verified it.
6. Removed the test rule after testing.

## Outcome
Learned how firewall rules control network traffic and how to allow or block specific ports.

## Interview Questions

### What is a firewall?
A firewall is a security system that monitors and filters incoming and outgoing network traffic based on predefined rules.

### Difference between stateful and stateless firewall?
- Stateful: Tracks active connections and makes decisions based on connection state.
- Stateless: Filters packets individually without tracking sessions.

### What are inbound and outbound rules?
- Inbound rules control incoming traffic.
- Outbound rules control outgoing traffic.

### How does UFW simplify firewall management?
UFW provides simple commands for managing firewall rules without complex configuration.

### Why block port 23 (Telnet)?
Telnet sends data in plain text and is insecure.

### Common firewall mistakes?
- Allowing unnecessary ports.
- Using overly broad rules.
- Forgetting to review logs.

### How does a firewall improve security?
It blocks unauthorized access and reduces attack surface.

### What is NAT in firewalls?
Network Address Translation hides internal IP addresses behind a public IP.

## Deliverables
- README.md
- Firewall configuration documentation
- Screenshots (to be added by the user)

