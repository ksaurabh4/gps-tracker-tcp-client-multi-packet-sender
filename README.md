# TCP Client for Sending Hex Data

This script is designed to send multiple hex-encoded data packets to a TCP server over the same connection. It can optionally receive and print responses from the server.

## Features

- Sends multiple hex data packets over the same TCP connection.
- Optionally receives and prints responses from the server.
- Includes timeout handling for receiving responses.
- Automatically closes the socket after sending all packets.

## How to Use

### Option 1: Run on Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Copy and paste the Python code (provided below) into a new notebook.
3. Replace the **`ip`**, **`port`**, and **`hex_data_list`** values in the code with your own.
4. Click on the "Run" button to execute the script.

If you'd prefer to use the pre-existing Colab notebook, you can [click here to open the notebook](https://colab.research.google.com/drive/1-lxmNV8_j7CabMejA8QAkFrjJ4GSurdx). *(Update this link with your Colab notebook URL once saved and shared)*.

### Option 2: Run Locally

1. Save the script in a Python file (e.g., `tcp_client.py`).
2. Open a terminal or command prompt.
3. Navigate to the directory where you saved the script.
4. Run the script using Python:

```bash
python TCP_client.py
```

For example:

```python
ip = '192.168.1.100'  # Replace with the server's IP address
port = 5005           # Replace with the server's port
hex_data_list = [
    '78780D01086471700328358100093F040D0A',
    '78781f121809030e1620c6027917540c4679500f142101cc00243c003e4a027fb7ac0d0a'
]

