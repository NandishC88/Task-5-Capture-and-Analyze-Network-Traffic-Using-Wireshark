**Objective**

To capture live network packets and identify basic protocols and traffic types using the Wireshark tool.

**Tools Used**

Software: Wireshark (Free Network Protocol Analyzer)

System Requirement: Windows 10 with active internet connection

**Procedure**

**Installation:**
Wireshark was downloaded from the official website and installed. During installation, the Npcap driver was enabled to allow live packet capture.

**Starting Capture:**
Wireshark was opened and the active Wi-Fi network interface was selected. The “Start Capturing Packets” button was clicked to begin monitoring live traffic.

**Generating Traffic:**
To create network activity, several websites such as google.com and example.com were visited, and the command ping google.com was run from Command Prompt to produce ICMP packets.

**Stopping Capture:**
After approximately one minute, the packet capture was stopped by pressing the red stop icon in Wireshark.

**Filtering Packets:**
The following display filters were applied to analyze specific protocol data:

http — to view HTTP packets

dns — to view DNS query and response packets

tcp — to analyze transport-level packets

**Identifying Protocols:**
At least three distinct protocols were observed during the session:

DNS (Domain Name System): Used to resolve domain names to IP addresses.

TCP (Transmission Control Protocol): Handles reliable data transport between client and server.

HTTP (Hypertext Transfer Protocol): Used for web page requests and responses.

**Exporting Data:**
The captured data was exported and saved as a .pcap file named network_capture.pcap for documentation and further analysis.

**Analysis Summary:**

Total packets captured: Approximately 250–300

Major protocols identified: HTTP, DNS, TCP, ICMP

The flow of data observed: DNS query → TCP handshake → HTTP data transfer

Communication pattern: Multiple small packets for DNS and TCP setup, larger packets for HTTP data

**Findings**

The analysis showed that before any HTTP request, DNS queries are sent to resolve domain names.

TCP connections are established between the client and the web server before the actual data (HTTP content) is transferred.

Most packets were TCP-based, showing that it is the backbone of reliable network communication.

**Conclusion**

This experiment provided practical exposure to network traffic monitoring and protocol analysis.
Using Wireshark, various protocols like DNS, TCP, and HTTP were identified, and their interactions were observed.
The task enhanced understanding of how data travels across the network and the role of each protocol in ensuring proper communication.

**Outcome**

Hands-on experience was gained in:

Capturing and filtering network packets

Understanding protocol layers and interactions

Exporting and documenting captured data
