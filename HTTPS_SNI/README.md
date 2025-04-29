# HTTPS SNI Test Configuration

This test implements HTTPS communication with Server Name Indication (SNI) support between a client and server.

## Configuration Template

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "ip": "TO_DO",
  "port": "TO_DO",
  "identifier": "TO_DO",
  "domain": "TO_DO",
  "request-data": {
    "host": "TO_DO",
    "method": "TO_DO",
    "path": "TO_DO",
    "headers": [
      ["TO_DO", "TO_DO"]
    ],
    "body": "TO_DO"
  },
  "response-data": {
    "method": "TO_DO",
    "path": "TO_DO",
    "status_code": "TO_DO",
    "headers": [
      ["TO_DO", "TO_DO"]
    ],
    "body": "TO_DO"
  }
}
```

## Explanation of Variables

- **role**: Specifies the role of the entity in the test. Can be either "client" or "server". Replace "TO_DO" with the appropriate role.
- **client**: Indicates the client entity in the test.
- **server**: Indicates the server entity in the test.
- **controller_conf_filename**: The name of the configuration file (in JSON format) containing settings for the control channel synchronization. Default is "controller_configuration.json".
- **ip**: The IP address of the server to connect to. Replace "TO_DO" with the server's IP address.
- **port**: The port number for the HTTPS connection. Replace "TO_DO" with your desired port number.
- **identifier**: The IP address or hostname used for generating the self-signed certificate. Replace "TO_DO" with the server's IP address or hostname.
- **domain**: The domain name to use in the SNI extension. Replace "TO_DO" with the target domain name.
- **request-data**: Configuration for the HTTP request:
  - **host**: The hostname to use in the request. Replace "TO_DO" with the target hostname.
  - **method**: The HTTP method to use (e.g., "GET", "POST"). Replace "TO_DO" with the desired method.
  - **path**: The resource path to request. Replace "TO_DO" with the desired path.
  - **headers**: Array of key-value pairs for HTTP request headers. Replace "TO_DO" with appropriate header names and values.
  - **body**: The request body content. Replace "TO_DO" with the desired body content.
- **response-data**: Configuration for the HTTP response:
  - **method**: The HTTP method (e.g., "GET"). Replace "TO_DO" with the appropriate method.
  - **path**: The requested resource path. Replace "TO_DO" with the appropriate path.
  - **status_code**: The HTTP status code to return. Replace "TO_DO" with the desired status code.
  - **headers**: Array of key-value pairs for HTTP response headers. Replace "TO_DO" with appropriate header names and values.
  - **body**: The response body content. Replace "TO_DO" with the desired response content.

