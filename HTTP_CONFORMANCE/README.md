## Overview

The purpose of this test is to detect non-conformance between a client and a server during HTTP communication.

## Test Variables Structure

The test relies on a set of variables to configure the client-server communication and to monitor the exchange of packets. Below is the JSON structure used for the variables:

### HTTP/1.1

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "ip": "TO_DO",
  "port": "TO_DO",
  "request-data": {
    "headers": [
      ["TO_DO", "TO_DO"],
    ],
    ":method": "TO_DO",
    ":path": "TO_DO",
    ":scheme": "TO_DO",
    ":authority": "TO_DO",
    "body": "TO_DO"
  },
  "response-data": {
    "path": "TO_DO",
    "method": "TO_DO",
    "status_code": "TO_DO",
    "headers": [
      ["TO_DO", "TO_DO"],
    ],
    "body": "TO_DO"
  }
}
```

### Explanation of Variables

- **role**: Specifies the role of the entity in the test. It can either be `client` or `server`. This helps in distinguishing between the actions and expectations from each side of the communication. Replace `TO_DO` with the role of the entity in the test.

- **client**: Indicates that the entity with this role is the client in the test.

- **server**: Indicates that the entity with this role is the server in the test.

- **controller_conf_filename**: The name of the configuration file (in JSON format) that contains additional settings or parameters required for the control channel synchronizing the workers. The default filename is `controller_configuration.json`.

- **ip**: The IP address of the server. This should be configured to match the server's actual IP address in the test environment. Replace `TO_DO` with the actual IP address.

- **port**: The port number on which the server is listening for incoming TCP connections. This should be configured to match the server's actual port number in the test environment. Replace `TO_DO` with the actual port number.

- **request-data**: A dictionary of fields that make up the HTTP request packet.

- **host**: Specifies the hostname or IP address of the server to which the HTTP request is being sent. 

- **path**: defines the specific resource or endpoint on the server being requested.

- **method**: Indicates the type of request being made.

- **body**: Contains the body of the HTTP request.

- **headers**: Array of key-value pairs that represent the HTTP headers sent with the request.

- **response-data**: Array of key-value pairs that represent the HTTP headers sent with the request.

- **status_code**: represents the HTTP status code returned by the server in response to the request.

### HTTP/2.0

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "ip": "TO_DO",
  "port": "TO_DO",
  "request-data": {
    "headers": [
      ["TO_DO", "TO_DO"],
    ],
    ":method": "TO_DO",
    ":path": "TO_DO",
    ":scheme": "http",
    ":authority": "TO_DO",
    "body": "TO_DO"
  },
  "response-data": {
    "path": "TO_DO",
    "method": "TO_DO",
    "status_code": "TO_DO",
    "headers": [
      ["TO_DO", "TO_DO"],
    ],
    "body": "TO_DO"
  }
}
```

### Explanation of Variables

- **role**: Specifies the role of the entity in the test. It can either be `client` or `server`. This helps in distinguishing between the actions and expectations from each side of the communication. Replace `TO_DO` with the role of the entity in the test.

- **client**: Indicates that the entity with this role is the client in the test.

- **server**: Indicates that the entity with this role is the server in the test.

- **controller_conf_filename**: The name of the configuration file (in JSON format) that contains additional settings or parameters required for the control channel synchronizing the workers. The default filename is `controller_configuration.json`.

- **ip**: The IP address of the server. This should be configured to match the server's actual IP address in the test environment. Replace `TO_DO` with the actual IP address.

- **port**: The port number on which the server is listening for incoming TCP connections. This should be configured to match the server's actual port number in the test environment. Replace `TO_DO` with the actual port number.

- **request-data**: A dictionary of fields that make up the HTTP request packet.

- **:authority**: Specifies the hostname or IP address of the server to which the HTTP request is being sent. 

- **:path**: Defines the specific resource or endpoint on the server being requested.

- **:scheme**: Specifies the protocol over which the request is made.

- **:method**: Indicates the type of request being made.

- **body**: Contains the body of the HTTP request.

- **headers**: Array of key-value pairs that represent the HTTP headers sent with the request.

- **response-data**: Array of key-value pairs that represent the HTTP headers sent with the request.

- **:status**: Represents the HTTP status code returned by the server in response to the request.