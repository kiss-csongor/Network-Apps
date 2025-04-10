# Network Device Discovery and Visualization

This is a Python-based tool for discovering network devices and visualizing network topologies. The application uses ARP requests for device discovery on the local network, retrieves LLDP (Link Layer Discovery Protocol) information from network devices via SSH, and generates a graphical network map.

## Features

1. **Network Interface Discovery**  
   The application retrieves available network interfaces, their IP addresses, subnets, and network masks.

2. **ARP-based Device Discovery**  
   The tool performs ARP (Address Resolution Protocol) scans to discover active devices on the network, collecting their IP and MAC addresses.

3. **SSH Connections and LLDP Information**  
   SSH connections are established to network devices (e.g., switches), and LLDP neighbor tables are retrieved. This information is saved to files.

4. **Network Graph Visualization**  
   The discovered devices are represented in a network graph, which visually depicts the devices and their connections, with icons representing different device types (e.g., PC, switch).

## Requirements

Before running the tool, you will need Python 3.x and the following Python libraries:

- `scapy` - For sending and receiving network packets.
- `psutil` - For retrieving network interface information.
- `paramiko` - For establishing SSH connections.
- `networkx` - For creating and managing network graphs.
- `matplotlib` - For visualizing the network graph.
- `Pillow` (PIL) - For handling device icons (e.g., PC, switch).

## Setting Up the Virtual Environment

Follow these steps to set up a Python virtual environment and install the required dependencies:

### 1. Create a Virtual Environment

First, navigate to the project directory in your terminal, then run the following command to create a virtual environment:

```bash
python -m venv env
