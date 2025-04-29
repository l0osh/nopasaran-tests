## Overview

The purpose of this test is to determine how many UDP packets sent by a sender (client) are authorized (i.e., allowed through the network) and successfully received by a receiver (server) within a short period of time.

## Test Variables Structure

The test is configured using a set of variables defined in JSON format. These variables control the roles, communication parameters, and coordination between client and server instances:

```json
{
  "role": "TO_DO",
  "client": "client",
  "server": "server",
  "controller_conf_filename": "controller_configuration.json",
  "server_ip": "TO_DO",
  "source_port": "TO_DO",
  "destination_port": "TO_DO",
  "batch_size": "TO_DO",
  "num_batches": "TO_DO",
  "delay": "TO_DO",
  "timeout": "TO_DO",
  "payload": "TO_DO"
}
```

### Explanation of Variables

- **role**: Defines whether the instance acts as the `"client"` (sender) or `"server"` (receiver).

- **client**: Identifies the entity responsible for sending UDP packets.

- **server**: Identifies the entity responsible for receiving and counting UDP packets.

- **controller_conf_filename**: Name of the controller configuration file that synchronizes client and server (default is `"controller_configuration.json"`).

- **server_ip**: IP address of the server to which UDP packets should be sent.

- **source_port**: UDP source port used by the client.

- **destination_port**: UDP destination port expected at the server.

- **batch_size**: The number of UDP packets to send in each batch.

- **num_batches**: The number of batches to send. Each batch will contain batch_size packets, and the test will run for the specified number of batches.

- **delay**: The time delay (in seconds) to wait between batches of UDP packets.

- **timeout**: The duration in seconds that the server will wait for incoming probes before timing out. This prevents indefinite waiting periods.

- **payload**: The data content that each UDP packet will carry. This can be used to define the size or content of the UDP packets being sent.

### Timing Constraint

**Important**: The product of `delay` and `batch_size` (`delay * batch_size`) or the `timeout` — whichever is greater — must not exceed the synchronization timeout defined in `EXCHANGE_SYNC.json`.
