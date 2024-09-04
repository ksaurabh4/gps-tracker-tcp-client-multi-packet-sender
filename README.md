# TCP Client for Sending Hex Data

This script is designed to send multiple hex-encoded data packets to a TCP server over the same connection. It can optionally receive and print responses from the server.

## Features

- Sends multiple hex data packets over the same TCP connection.
- Optionally receives and prints responses from the server.
- Includes timeout handling for receiving responses.
- Automatically closes the socket after sending all packets.

## How to Use

### Step 1: Set Up the Python Environment

Make sure Python is installed on your system. This code uses the built-in `socket` and `time` libraries, so no additional packages are needed.

### Step 2: Modify the IP, Port, and Data

In the script, replace the following values:

- **`ip`**: The IP address of the TCP server.
- **`port`**: The port number of the TCP server.
- **`hex_data_list`**: A list of hex strings you want to send.

For example:

```python
ip = '192.168.1.100'  # Replace with the server's IP address
port = 5005           # Replace with the server's port
hex_data_list = [
    '78780D01086471700328358100093F040D0A',
    '78781f121809030e1620c6027917540c4679500f142101cc00243c003e4a027fb7ac0d0a'
]

