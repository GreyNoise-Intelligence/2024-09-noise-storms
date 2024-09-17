# 2024-09-noise-storms

Notes and receipts (PCAPs) for TCP and ICMP Noise Storms

See [this episode of Storm⚡️Watch](https://www.greynoise.io/storm-watch-episodes/andrew-morris-on-noise-storms-uncovering-a-hidden-message-in-millions-of-icmp-packets) for more information.

- `brazil-storm-small-tcp-sample/`: sample of a TCP Noise Storm mentioned in the episode
- `noise-storm-icmp-brazil/`: full capture of the ICMP Noise Storm mentioned in the episode

## Background (from the episode)

1. Noise Storms are large-scale spoofed packet events first observed in January 2020, coinciding with the U.S. military action against Iranian General Soleimani.

2. They involve millions of spoofed IP addresses, primarily appearing to originate from Brazil in recent months.

3. The traffic is mostly TCP (port 443) and ICMP, with no UDP traffic observed.

4. Recent ICMP packets contain the ASCII string "LOVE" embedded in them, along with other varying bytes.

5. TTLs are intelligently spoofed, typically between 120 and 200.

6. The storms have evolved to be more targeted, hitting smaller parts of the internet but with increased intensity.

7. They often coincide with significant geopolitical or military events.

8. The TCP traffic intelligently spoofs window sizes to mimic packets from various operating systems.

9. Recent storms have avoided AWS but hit other providers like Cogent, Lumen, and Hurricane Electric.

10. The ASN for the ICMP traffic is associated with a CDN organization servicing QQ, WeChat, and WePay.

11. Possible theories include covert communications, DDoS attempts, misconfigured routers, command and control mechanisms, or attempts to create network congestion for traffic manipulation.

12. The purpose and origin of these Noise Storms remain unknown despite ongoing investigation for over four years.
