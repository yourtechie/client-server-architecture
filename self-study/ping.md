# Understanding Ping and Traceroute Network Diagnostic Utilities

## Ping
**Ping** is a network diagnostic tool used to test the reachability of a host on an IP network. It measures the round-trip time for messages sent from the originating host to a destination computer.

**How Ping Works:**
- Ping uses the Internet Control Message Protocol (ICMP) to send echo request packets to the target host and waits for an echo reply.
- The command provides information about the time taken for the round trip and any packet loss.

**Example:**
```bash
ping google.com
```
Output:
```
PING google.com (172.217.10.46): 56 data bytes
64 bytes from 172.217.10.46: icmp_seq=0 ttl=56 time=15.740 ms
64 bytes from 172.217.10.46: icmp_seq=1 ttl=56 time=14.648 ms
64 bytes from 172.217.10.46: icmp_seq=2 ttl=56 time=11.153 ms
64 bytes from 172.217.10.46: icmp_seq=3 ttl=56 time=12.577 ms
64 bytes from 172.217.10.46: icmp_seq=4 ttl=56 time=22.400 ms
64 bytes from 172.217.10.46: icmp_seq=5 ttl=56 time=12.620 ms
--- google.com ping statistics ---
6 packets transmitted, 6 packets received, 0.0% packet loss
round-trip min/avg/max/stddev = 11.153/14.856/22.400/3.689 ms
```
**Interpreting Results:**
- **Packets Transmitted/Received:** Indicates the number of packets sent and received.
- **Packet Loss:** Shows the percentage of packets lost during transmission.
- **Round-Trip Time (RTT):** Provides the minimum, average, maximum, and standard deviation of the round-trip times.

