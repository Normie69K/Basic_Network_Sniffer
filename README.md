#  Basic Network Sniffer

## Overview

The **Basic Network Sniffer** is a Python-based tool that captures and analyzes network traffic. It provides insights into Ethernet frames, IPv4 packets, ICMP, and TCP segments, making it a great resource for learning about network protocols and packet structures. This tool is ideal for networking enthusiasts, cybersecurity learners, and ethical hackers.

---

## Features

- **Packet Capture**:
  - Captures raw network traffic in real-time using `socket`.
  - Displays Ethernet, IPv4, ICMP, and TCP packet details.
- **Protocol Analysis**:
  - Parses Ethernet frames to extract MAC addresses and protocol types.
  - Decodes IPv4 packets, including TTL, source, and destination IPs.
  - Unpacks and analyzes ICMP and TCP headers.
- **Custom Formatting**:
  - Formats multi-line data for better readability during analysis.

---

## Prerequisites

Before running this tool, ensure you have the following:

1. **Python 3.x** installed on your system. [Download Python](https://www.python.org/downloads/)

2. Required Python modules:

   - `socket`
   - `struct`
   - `textwrap`

   These modules are part of Python's standard library, so no additional installation is necessary.

3. Administrator/root privileges (required for raw socket access).

4. A basic understanding of networking concepts is recommended.

---

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/Normie69K/CodeAlpha_Basic_Network_Sniffer.git
   ```

2. Navigate to the project directory:

   ```bash
   cd CodeAlpha_Basic_Network_Sniffer
   ```

---

## Usage

To start the network sniffer, run the following command:

```bash
sudo python network_sniffer.py
```

### Example Output

When running the tool, you will see output like:

```
Ethernet Frame:
Destination: AA:BB:CC:DD:EE:FF, Source: FF:EE:DD:CC:BB:AA, Protocol: 8

IPv4 Packet:
Version: 4, Header Length: 20, TTL: 64
Protocol: 1, Source: 192.168.1.1, Target: 192.168.1.2

ICMP Packet:
Type: 8, Code: 0, Checksum: 12345
```

---

## Project Structure

```
CodeAlpha_Basic_Network_Sniffer/
├── network_sniffer.py     # Main script for packet capturing
├── README.md              # Project documentation
└── LICENSE                # License file
```

---

## Known Limitations

- Currently supports Ethernet, IPv4, ICMP, and TCP protocols.
- No advanced filtering options (e.g., by IP address or port range).
- Does not save captured packets to files like `.pcap`.

---

## Potential Enhancements

- Add support for additional protocols (e.g., UDP, ARP).
- Implement packet filtering by source/destination IP or port.
- Save captured packets to `.pcap` format for analysis in Wireshark.
- Build a user-friendly GUI for non-technical users.

---

## Contributing

Contributions are welcome! Follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push to your forked repository.
4. Submit a pull request with a detailed description of your changes.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Disclaimer

This tool is intended for educational purposes only. Do not use it to sniff traffic on networks you do not own or have explicit permission to monitor.

---

