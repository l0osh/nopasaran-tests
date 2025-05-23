## Overview

This test checks if a specific DNS query name is banned or censored on the network.

## Test Variables Structure

The test relies on a set of variables to configure the client-server communication and to monitor DNS query behavior. Below is the JSON structure used for the variables:

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "ip": "TO_DO",
  "filter": "TO_DO",
  "qname": "TO_DO",
  "response_ip": "TO_DO"
}
```

### Explanation of Variables

- **role**: Specifies the role of the entity in the test. It can either be `client` or `server`. This helps in distinguishing between the actions and expectations from each side of the communication.

- **client**: Indicates that the entity with this role is the client in the test.

- **server**: Indicates that the entity with this role is the server in the test.

- **controller_conf_filename**: The name of the configuration file (in JSON format) that contains additional settings or parameters required for the control channel synchronizing the workers. The default filename is `controller_configuration.json`.

- **ip**: The IP address of the server. This should be configured to match the server's actual IP address in the test environment. Replace `TO_DO` with the actual IP address.

- **filter**: The filter expression used to capture and analyze network traffic. In this case, the filter is `TO_DO`, where `TO_DO` should match the BPF (Berkeley Packet Filter) expression that would be used to capture the relevant DNS packets.

- **qname**: The domain name being queried in the DNS request. This is the name being tested for possible censorship. Replace `TO_DO` with the actual domain name you want to check.

- **response_ip**: The IP address returned in the Resource Record (RR) section of the DNS response. Replace `TO_DO` with the IP address you expect or want to check against in the test.
