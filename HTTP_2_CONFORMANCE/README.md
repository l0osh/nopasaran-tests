## Overview

The purpose of this test is to detect non-conformance between a client and a server during HTTP communication.

## Test Variables Structure

The test relies on a set of variables to configure the client-server communication and to monitor the exchange of packets. Below is the JSON structure used for the variables:

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "host": "TO_DO",
  "port": "TO_DO",
  "tls_enabled": "TO_DO",
  "protocol": "TO_DO",
  "connection_settings_server": {"TO_DO": "TO_DO"},
  "connection_settings_client": {"TO_DO": "TO_DO"},
  "client_frames": [
      {
          "type": "TO_DO",
          "tests": [
              [
                  {
                      "function": "TO_DO",
                      "params": [
                          "TO_DO"
                      ]
                  }
              ]
          ]
      }
  ],
  "server_frames": [
      {
          "type": "TO_DO",
          "tests": [
              [
                  {
                      "function": "TO_DO",
                      "params": [
                          "TO_DO"
                      ]
                  }
              ]
          ]
      }
  ]
}
```

### Explanation of Variables

- **role**: Specifies the role of the entity in the test. It can either be `client` or `server`. This helps in distinguishing between the actions and expectations from each side of the communication. Replace `TO_DO` with the role of the entity in the test.

- **client**: Indicates that the entity with this role is the client in the test.

- **server**: Indicates that the entity with this role is the server in the test.

- **controller_conf_filename**: The name of the configuration file (in JSON format) that contains additional settings or parameters required for the control channel synchronizing the workers. The default filename is `controller_configuration.json`.

- **host**: The IP address of the server. This should be configured to match the server's actual IP address in the test environment. Replace `TO_DO` with the actual IP address.

- **port**: The port number on which the server is listening for incoming TCP connections. This should be configured to match the server's actual port number in the test environment. Replace `TO_DO` with the actual port number.

- **tls_enabled**: Indicates whether TLS encryption is enabled for the server. Replace `TO_DO` with the actual value.

- **protocol**: The protocol used for the HTTP communication. Replace `TO_DO` with the actual protocol.

- **connection_settings_server**: A dictionary of fields change how the server will be configured.

- **connection_settings_client**: A dictionary of fields change how the client will be configured.

- **client_frames**: A list of frames that the client will send.
  - **type**: The type of frame.
  - **tests**: A list of tests that the client will perform.
    - **function**: The function to be tested.
    - **params**: The parameters to be passed to the function.

- **server_frames**: A list of frames that the server will send.