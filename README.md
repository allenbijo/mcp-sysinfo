# MCP System Info Server

## Overview
The **MCP System Info Server** is a lightweight and efficient server that provides real-time system information. It retrieves various hardware and system details, including CPU, memory, disk, and GPU statistics, making it useful for monitoring and diagnostic purposes.

## Features
- **System Information**
  - System Name
  - Node Name
  - OS Release
  - OS Version
  - Machine Type
  - Processor
- **CPU Information**
  - Processor Name
  - Physical Cores
  - Logical Cores
- **Memory Information**
  - Total Memory
  - Available Memory
  - Used Memory
  - Memory Utilization
- **Disk Information**
  - Total Disk Space
  - Used Disk Space
  - Free Disk Space
  - Disk Space Utilization
- **GPU Information**
  - GPU ID
  - GPU Name
  - Driver Version
  - Total GPU Memory
  - Free GPU Memory
  - Used GPU Memory
  - GPU Load
  - GPU Temperature

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/allenbijo/mcp-sysinfo.git
   ```

## Usage
Add the MCP server to your client:

On Claude
```sh
{
  "mcpServers": {
    "sysinfo": {
      "command": "uv",
      "args": [
          "--directory",
          "D:\\WorksOfGreatness\\mcp-sysinfo",
          "run",
          "sysinfo.py"
      ]
    }
  }
}
```
The server will start and listen for incoming requests, providing real-time system information.

## API Endpoints
| Endpoint       | Description               |
|--------------|--------------------------|
|`/get_sysinfo`| Returns system details   |


## License
This project is licensed under the MIT License.


## Author
Allen Bijo - [GitHub](https://github.com/allenbijo)

