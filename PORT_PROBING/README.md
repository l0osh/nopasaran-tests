# Port Probing Module

This module implements a comprehensive port scanning mechanism that can probe both TCP and UDP ports across all possible destination ports. It supports both client and server roles, with the client initiating the probes and the server listening for and responding to them.

## Overview

The purpose of this test is to verify the integrity of port scanning operations across all possible destination ports. The state machine implements both TCP SYN scanning and UDP port scanning, allowing for comprehensive port availability testing between a client and server.

## Test Variables Structure

The test is configured through a set of variables defined in JSON format. These variables determine the roles, the communication protocol, and the addressing information:

```json
{
  "role": "TO_DO",
  "client": "TO_DO",
  "server": "TO_DO",
  "controller_conf_filename": "TO_DO",
  "protocol": "TO_DO",
  "client_ip": "TO_DO",
  "server_ip": "TO_DO",
  "timeout": "TO_DO"
}
```

### Explanation of Variables

- **role**: Indicates the role of the current test instance. It should be set to either `"client"` or `"server"` depending on which side of the communication is being configured.

- **client**: Identifies the entity responsible for sending a single probe packet to the server.

- **server**: Identifies the receiving entity, responsible for capturing and validating the incoming probe packet.

- **controller_conf_filename**: The name of the controller configuration file (default is `"conf_endpoint.json"`). This file provides synchronization and parameter control for the client and server instances involved in the test.

- **protocol**: Specifies the transport layer protocol used for port scanning. Acceptable values are `"tcp"` or `"udp"`. This determines whether TCP SYN scanning or UDP port scanning is performed.

- **client_ip**: The IP address of the client to accept connections from. This ensures the listener filters the incoming probes based on the client's IP address.

- **server_ip**: The target IP address to scan. This is the destination address where the port scanning will be performed.

- **timeout**: The duration in seconds that the server will wait for incoming probes before timing out. This prevents indefinite waiting periods.
