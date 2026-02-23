## Day 1 Wireshark Observations

### DNS Packet
- DNS server IP found: 81.50.109.10
- Layer 4 protocol used: UDP
- Port number: 53

### TCP Handshake
- Found it: Yes
- Observations:
  - SYN → Client says "I want to connect, here is my sequence number"
  - SYN-ACK → Server says "Accepted. I acknowledge your sequence, here is mine"
  - ACK → Client says "Acknowledged. Connection established."

### ICMP
- Found it: No
- Reason: No pinging occurred during the session