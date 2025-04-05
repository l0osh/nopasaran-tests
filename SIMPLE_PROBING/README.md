## Overview

The purpose of this test is to verify the integrity of single probe packets sent from a client to a server over TCP or UDP. The state machine checks whether these packets are received by the server and whether any fields at the IP or TCP layer have been altered during transmission.

## Test Variables Structure

The test is configured through a set of variables defined in JSON format. These variables determine the roles, the communication protocol, the addressing information, and how traffic is captured and analyzed:

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "conf_endpoint.json",
  "protocol": "tcp",
  "src_ip": "TO_DO",
  "dst_ip": "TO_DO",
  "sport": "TO_DO",
  "dport": "TO_DO",
  "filter": "TO_DO"
}
```

### Explanation of Variables

- **role**: Indicates the role of the current test instance. It should be set to either `"client"` or `"server"` depending on which side of the communication is being configured.

- **client**: Identifies the entity responsible for sending a single probe packet to the server.

- **server**: Identifies the receiving entity, responsible for capturing and validating the incoming probe packet.

- **controller_conf_filename**: The name of the controller configuration file (default is `conf_endpoint.json`). This file provides synchronization and parameter control for the client and server instances involved in the test.

- **protocol**: Specifies the transport layer protocol used for the probe packet. Acceptable values are `"tcp"` or `"udp"`. This determines how the packet is constructed and which headers are analyzed for modification.

- **src_ip**: The source IP address used in the probe packet. If the value is `"self"`, the test uses the actual IP of the client, indicating that IP spoofing is not being tested. Otherwise, this value should be set to a specific IP address to test IP spoofing.

- **dst_ip**: The destination IP address of the server to which the probe packet is sent.

- **sport**: The source port number used by the client. Relevant for both TCP and UDP.

- **dport**: The destination port number on the server expected to receive the probe packet.

- **filter**: A packet capture filter expression (e.g., `udp dst port 1234` or `tcp dst port 80`) that isolates relevant traffic for analysis. This ensures that only packets matching the specified protocol and ports are evaluated by the state machine.
