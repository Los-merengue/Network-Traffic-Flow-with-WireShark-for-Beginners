# Analyzing DNS, TCP, HTTP and TLS Traffic with Wireshark

## Introduction

In this project, you'll learn how to use Wireshark to capture and analyze DNS, TCP, HTTP, and TLS traffic. Traffic analysis is crucial for understanding network communication, identifying potential security issues, troubleshooting network problems, and investigating anomalies in network traffic.

## Pre-requisites

- Basic understanding of networking concepts
- Wireshark installed on your computer
- A web browser for generating network traffic
- Basic understanding of DNS, TCP, HTTP, and TLS

## Lab Set-up and Tools

1. **Wireshark**: Download and install Wireshark from [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html).
2. **Web Browser**: Any modern web browser (e.g., Chrome, Firefox) for generating network traffic.

## Exercises

### Exercise 1: Capture DNS Traffic

#### Steps

1. Open Wireshark.
2. Select the network interface that connects to the internet.
3. Click on the "Start Capture" button (the blue shark fin icon).
4. Open your web browser and navigate to a website (e.g., https://example.com).
5. Let the page load completely and then stop the capture in Wireshark by clicking on the red square icon.

#### Expected Output

- A capture file containing network traffic, including DNS queries and responses.

### Exercise 2: Filter DNS Traffic

#### Steps

1. In Wireshark, go to the filter bar at the top.
2. Enter the filter `dns` and press Enter.
3. Wireshark will display only the DNS traffic from the capture.

#### Expected Output

- Displayed DNS traffic filtered from the overall capture.

### Exercise 3: Analyze DNS Requests

#### Steps

1. In the filtered DNS traffic, locate a DNS query.
2. Click on the DNS query to view its details in the packet details pane.
3. Expand the "Domain Name System" section to see detailed information about the request, such as the queried domain name and query type.

#### Expected Output

- Detailed information about a DNS query displayed.

### Exercise 4: Analyze DNS Responses

#### Steps

1. In the filtered DNS traffic, locate the corresponding DNS response for the query you analyzed.
2. Click on the response to view its details in the packet details pane.
3. Expand the "Domain Name System" section to see information about the response, such as the response code and returned IP address.

#### Expected Output

- Detailed information about a DNS response displayed.

### Exercise 5: Examine DNS Traffic

#### Steps

1. In the DNS response details, look for the returned IP address.
2. Identify the source and destination IP addresses of the DNS communication.
3. Examine the DNS query and response to understand how the domain name was resolved.

#### Expected Output

- DNS query and response information examined and documented.

---

### Exercise 6: Capture TCP Traffic

#### Steps

1. Open Wireshark.
2. Select the network interface that connects to the internet.
3. Click on the "Start Capture" button.
4. Open your web browser and navigate to a website (e.g., https://example.com).
5. Let the page load completely and then stop the capture in Wireshark by clicking on the red square icon.

#### Expected Output

- A capture file containing network traffic, including TCP connections.

### Exercise 7: Filter TCP Traffic

#### Steps

1. In Wireshark, go to the filter bar at the top.
2. Enter the filter `tcp` and press Enter.
3. Wireshark will display only the TCP traffic from the capture.

#### Expected Output

- Displayed TCP traffic filtered from the overall capture.

### Exercise 8: Analyze the TCP Three-Way Handshake

#### Steps

1. In the filtered TCP traffic, locate a TCP SYN packet.
2. Click on the SYN packet to view its details in the packet details pane.
3. Locate the corresponding SYN-ACK packet.
4. Locate the final ACK packet.
5. Examine the TCP flags and sequence information in each packet.

#### Expected Output

- Detailed information about the TCP three-way handshake displayed.

### Exercise 9: Analyze TCP Connections

#### Steps

1. Select one of the TCP packets from the filtered traffic.
2. Identify the source and destination IP addresses.
3. Identify the source and destination ports.
4. Expand the "Transmission Control Protocol" section to examine TCP information such as flags, sequence numbers, and acknowledgment numbers.

#### Expected Output

- Detailed information about a TCP connection displayed.

### Exercise 10: Follow a TCP Stream

#### Steps

1. Right-click on a TCP packet.
2. Select "Follow" > "TCP Stream".
3. Examine the packets exchanged between the client and server.
4. Review the stream to understand the communication between the two systems.

#### Expected Output

- TCP stream showing the communication between the client and server.

---

### Exercise 11: Capture HTTP Traffic

#### Steps

1. Open Wireshark.
2. Select the network interface that connects to the internet.
3. Click on the "Start Capture" button (the blue shark fin icon).
4. Open your web browser and navigate to a website that uses HTTP (e.g., http://example.com).
5. Let the page load completely and then stop the capture in Wireshark by clicking on the red square icon.

#### Expected Output

- A capture file containing network traffic, including HTTP requests and responses.

### Exercise 12: Filter HTTP Traffic

#### Steps

1. In Wireshark, go to the filter bar at the top.
2. Enter the filter `http` and press Enter.
3. Wireshark will display only the HTTP traffic from the capture.

#### Expected Output

- Displayed HTTP traffic filtered from the overall capture.

### Exercise 13: Analyze HTTP Requests

#### Steps

1. In the filtered HTTP traffic, locate an HTTP GET request.
2. Click on the GET request to view its details in the packet details pane.
3. Expand the "Hypertext Transfer Protocol" section to see detailed information about the request, such as the requested URL, headers, and parameters.

#### Expected Output

- Detailed information about an HTTP GET request displayed.

### Exercise 14: Analyze HTTP Responses

#### Steps

1. In the filtered HTTP traffic, locate the corresponding HTTP response for the GET request you analyzed.
2. Click on the response to view its details in the packet details pane.
3. Expand the "Hypertext Transfer Protocol" section to see detailed information about the response, such as the status code, headers, and content type.

#### Expected Output

- Detailed information about an HTTP response displayed.

### Exercise 15: Extract and Examine Payload Data

#### Steps

1. In the HTTP response details, look for the payload data (e.g., HTML content).
2. Right-click on the response packet and select "Follow" > "TCP Stream" to view the entire HTTP conversation.
3. Examine the payload data in the TCP stream window to understand the content being transferred.

#### Expected Output

- Payload data from the HTTP response extracted and examined.

---

### Exercise 16: Capture TLS Traffic

#### Steps

1. Open Wireshark.
2. Select the network interface that connects to the internet.
3. Click on the "Start Capture" button (the blue shark fin icon).
4. Open your web browser and navigate to a website that uses HTTPS (e.g., https://example.com).
5. Let the page load completely and then stop the capture in Wireshark by clicking on the red square icon.

#### Expected Output

- A capture file containing network traffic, including TLS handshake and encrypted traffic.

### Exercise 17: Filter TLS Traffic

#### Steps

1. In Wireshark, go to the filter bar at the top.
2. Enter the filter `tls` and press Enter.
3. Wireshark will display only the TLS traffic from the capture.

#### Expected Output

- Displayed TLS traffic filtered from the overall capture.

### Exercise 18: Analyze TLS Client Hello

#### Steps

1. In the filtered TLS traffic, locate a "Client Hello" packet.
2. Click on the Client Hello packet to view its details in the packet details pane.
3. Expand the "Transport Layer Security" section.
4. Examine information such as the TLS version, supported cipher suites, and extensions.

#### Expected Output

- Detailed information about a TLS Client Hello packet displayed.

### Exercise 19: Analyze TLS Server Hello

#### Steps

1. In the filtered TLS traffic, locate the corresponding "Server Hello" packet.
2. Click on the Server Hello packet to view its details in the packet details pane.
3. Expand the "Transport Layer Security" section.
4. Examine information such as the selected TLS version and cipher suite.

#### Expected Output

- Detailed information about a TLS Server Hello packet displayed.

### Exercise 20: Examine TLS Certificates

#### Steps

1. In the filtered TLS traffic, locate a packet containing certificate information.
2. Click on the packet to view its details in the packet details pane.
3. Expand the certificate-related section.
4. Examine available information such as the certificate issuer, subject, and validity period.

#### Expected Output

- TLS certificate information identified and examined.

### Exercise 21: Examine Encrypted TLS Traffic

#### Steps

1. In the TLS traffic, locate packets exchanged after the TLS handshake.
2. Click on one of the packets to view its details.
3. Examine the encrypted application data.
4. Compare the encrypted traffic with the HTTP traffic analyzed earlier.

#### Expected Output

- Encrypted application traffic identified and examined.

## Conclusion

By completing these exercises, you have learned how to capture, filter, and analyze DNS, TCP, HTTP, and TLS traffic using Wireshark. These skills are essential for understanding network communication, troubleshooting network issues, identifying suspicious traffic, and performing security investigations.

The basic flow of a web connection can be summarized as:

**DNS → TCP → TLS → HTTP/HTTPS**