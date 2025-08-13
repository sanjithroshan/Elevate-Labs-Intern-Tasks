Wireshark Packet Capture & Analysis – Task Report
Installed Wireshark

Downloaded and installed Wireshark on Windows.

Installed Npcap to enable live packet capture.

Selected Active Network Interface

Identified Wi-Fi as the active interface using the live traffic graph.

Started packet capture on the Wi-Fi interface.

Generated Network Traffic

Opened Command Prompt and ran the command:
ping google.com
This generated DNS lookups and ICMP ping requests/replies to google.com.

Stopped Packet Capture

Captured traffic for approximately 1 minute.

Stopped capture using the red stop button in Wireshark.

Filtered Packets by Protocol

Applied filters to isolate specific protocols:

dns – Viewed domain resolution queries and responses.

tcp – Viewed TCP handshake and data transfer packets.

tls – Viewed encrypted HTTPS packets.

Identified Protocols in the Capture

DNS – Resolved google.com to IP address 142.250.182.174.

TCP – Showed SYN → SYN/ACK → ACK handshake between local machine and remote servers.

TLS – Encrypted HTTPS communication to Google services.

Exported Packet Capture

Saved the captured file in .pcapng format for submission and future analysis.

Summary of Findings

DNS resolves domain names before communication.

TCP establishes connections through a handshake process.

TLS secures web traffic through encryption.

Learned to apply protocol filters and interpret packet details.