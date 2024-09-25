# Traceroute

**Traceroute** is a network diagnostic tool used to track the path that a packet takes from the source to the destination. It helps identify where delays or failures occur in the network.

**How Traceroute Works:**
- Traceroute sends packets with gradually increasing Time-To-Live (TTL) values.
- Each router along the path decreases the TTL by 1 and, when the TTL reaches 0, the router sends an ICMP "Time Exceeded" message back to the source.
- This process continues until the packet reaches the destination or the maximum TTL is reached.

**Example:**
```bash
traceroute google.com
```
Output:
```
traceroute to google.com (172.217.10.46), 30 hops max, 60 byte packets
 1  192.168.1.1 (192.168.1.1)  1.123 ms  1.098 ms  1.073 ms
 2  10.0.0.1 (10.0.0.1)  2.345 ms  2.321 ms  2.297 ms
 3  172.217.10.46 (172.217.10.46)  14.567 ms  14.543 ms  14.519 ms
```
**Interpreting Results:**
- **Hops:** Each line represents a hop, or a router, that the packet passes through.
- **IP Address:** The IP address of each hop.
- **Round-Trip Time:** The time taken for the packet to reach each hop and return.

