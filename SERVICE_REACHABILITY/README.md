# Echo Server Reachability Test

## Overview

The purpose of this test is to verify **TCP/UDP service reachability** between a client and a server using echo socket communication. The server listens on the specified IP and port, and the client attempts to send messages using TCP or UDP, validating that responses are echoed back.

## Test Variables Structure

The test relies on a `variables.json` file to configure both the control channel and the communication protocol between the client and the server.

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "protocol": "TO_DO",
  "tcp": "TO_DO",
  "ip": "TO_DO",
  "port": "TO_DO",
  "payload": "TO_DO"
}
```

### Explanation of Variables

- **role**: Specifies whether this machine acts as a `client` or `server`. Determines branching behavior in the state machine. Replace `TO_DO` with the role of the entity in the test.

- **client**: Indicates that the entity with this role is the client in the test.

- **server**: Indicates that the entity with this role is the server in the test.

- **controller_conf_filename**: The name of the configuration file (in JSON format) that contains additional settings or parameters required for the control channel synchronizing the workers. The default filename is `controller_configuration.json`.

- **protocol**: Specifies the transport layer protocol used for the probe packet. Acceptable values are `"tcp"` or `"udp"`. This determines how the packet is constructed and which headers are analyzed for modification.

- **tcp**: Indicates that the protocol is tcp in this test.

- **ip**: The IP address of the server. This should be configured to match the server's actual IP address in the test environment. Replace `TO_DO` with the actual IP address.

- **port**: The port number on which the server is listening for incoming connections. This should be configured to match the server's actual port number in the test environment. Replace `TO_DO` with the actual port number.

- **payload**: The message body that the client sends. Replace `TO_DO` with the packet payload.

