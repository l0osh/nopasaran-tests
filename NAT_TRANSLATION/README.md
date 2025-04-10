## Overview

The purpose of this test is to identify the presence of NAT (Network Address Translation) and observe TCP port randomization behavior during client-server communication.

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
  "filter": "tcp port TO_DO"
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



