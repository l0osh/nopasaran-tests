## Overview

The purpose of this test is to detect sequence number discrepancies between a client and a server during TCP communication.

## Test Variables Structure

The test relies on a set of variables to configure the client-server communication and to monitor the exchange of packets. Below is the JSON structure used for the variables:

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "ip": "TO_DO",
  "port": "TO_DO",
  "filter": "tcp port TO_DO",
  "syn": "S",
  "ack": "A",
  "syn/ack": "SA"
}
```

### Explanation of Variables

- **role**: Specifies the role of the entity in the test. It can either be `client` or `server`. This helps in distinguishing between the actions and expectations from each side of the communication.

- **client**: Indicates that the entity with this role is the client in the test.

- **server**: Indicates that the entity with this role is the server in the test.

- **controller_conf_filename**: The name of the configuration file (in JSON format) that contains additional settings or parameters required for the control channel synchronizing the workers. The default filename is `controller_configuration.json`.

- **ip**: The IP address of the server. This should be configured to match the server's actual IP address in the test environment. Replace `TO_DO` with the actual IP address.

- **port**: The port number on which the server is listening for incoming TCP connections. This should be configured to match the server's actual port number in the test environment. Replace `TO_DO` with the actual port number.

- **filter**: The filter expression used to capture and analyze network traffic. In this case, the filter is `tcp port TO_DO`, where `TO_DO` should match the port number specified in the `port` variable. This ensures that only relevant TCP traffic is captured for analysis.

- **syn**: Represents the SYN (synchronize) flag in a TCP packet, which is used to initiate a TCP connection.

- **ack**: Represents the ACK (acknowledgment) flag in a TCP packet, used to acknowledge the receipt of data.

- **syn/ack**: Represents a TCP packet with both the SYN and ACK flags set, typically sent by the server in response to a SYN packet from the client.

