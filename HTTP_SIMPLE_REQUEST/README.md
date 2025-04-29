## Overview

The purpose of this test is to send HTTP(S) requests from two machines to a specific IP or hostname in order to check for discrepancies in reception between the client and the server.

## Test Variables Structure

The test relies on a set of variables to configure the client-server communication and monitor the exchange of packets. Below is the JSON structure used for the variables:

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "ip": "TO_DO",
  "hostname": "TO_DO",
  "use_https": "TO_DO"
}
```

### Explanation of Variables

- **role**: Specifies the role of the entity in the test. It can either be `client` or `server` for the control channel. This helps in distinguishing between the actions and expectations from each side of the communication. Replace `TO_DO` with the role of the entity in the control channel.

- **client**: The entity acting as the client in the control channel.

- **server**: The entity acting as the server in the control channel.

- **controller_conf_filename**: The name of the configuration file (in JSON format) that contains additional settings or parameters required for controlling the test execution. The default filename is `controller_configuration.json`.

- **ip**: The IP address of the server to which the client is sending the request.

- **hostname**: The hostname of the server.

- **use_https**: Specifies whether HTTPS is being used in the communication. The value can either be `"1"` (for HTTPS) or `"0"` (for HTTP).
