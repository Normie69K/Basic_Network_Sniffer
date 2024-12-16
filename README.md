# CodeAlpha Basic Network Sniffer

## Overview

The **CodeAlpha Basic Network Sniffer** is a Python-based tool that captures and analyzes network traffic. It is designed to provide insights into how data flows through a network and to help users understand packet structures, including Ethernet, IP, TCP, and UDP headers. This tool is an excellent starting point for those interested in networking, cybersecurity, or ethical hacking.

---

## Features

- **Packet Capture**:
  - Captures network packets in real-time.
  - Displays source and destination IP addresses, ports, and protocols.
- **Protocol Analysis**:
  - Supports TCP, UDP, and ICMP protocols.
  - Parses and displays detailed packet headers.
- **Filtering**:
  - Option to filter packets by protocol type.
- **Save to File**:
  - Export captured packets to `.pcap` files for further analysis.

---

## Prerequisites

Before running this tool, ensure you have the following:

1. **Python 3.x** installed on your system. [Download Python](https://www.python.org/downloads/)

2. Required Python modules:

   - `scapy`
   - `socket`

   Install them using pip:

   ```bash
   pip install scapy
   ```

3. Administrator/root privileges (required for packet capture).

4. A basic understanding of networking concepts is recommended.

---

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/CodeAlpha_Basic_Network_Sniffer.git
   ```

2. Navigate to the project directory:

   ```bash
   cd CodeAlpha_Basic_Network_Sniffer
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

To start the network sniffer, run the following command:

```bash
sudo python network_sniffer.py
```

### Command-Line Options

| Option            | Description                                  |
| ----------------- | -------------------------------------------- |
| `--protocol`      | Filter packets by protocol (e.g., TCP, UDP). |
| `--output <file>` | Save captured packets to a `.pcap` file.     |

Example:

```bash
sudo python network_sniffer.py --protocol tcp --output traffic.pcap
```

---

## Project Structure

```
CodeAlpha_Basic_Network_Sniffer/
├── network_sniffer.py     # Main script for packet capturing
├── README.md              # Project documentation
├── requirements.txt       # Python dependencies
└── LICENSE                # License file
```

---

## Screenshots

### Packet Capture in Action:



---

## Potential Enhancements

- Add support for HTTPS decryption (with proper permissions).
- Create a GUI for easier interaction.
- Implement advanced filtering options (e.g., by IP, port range).
- Integrate with tools like Wireshark for deeper analysis.

---

## Contributing

Contributions are welcome! Follow these steps:

1. Fork the repository.
2. Create a new branch for your feature/bug fix:
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

## Acknowledgments

Special thanks to **CodeAlpha** for inspiring this project and providing guidance on cybersecurity practices.

