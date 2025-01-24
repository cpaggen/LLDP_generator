# LLDP PDU Generator

This Python script generates and transmits LLDP (Link Layer Discovery Protocol) PDUs. It can be used for various purposes, such as network discovery or testing LLDP implementations.

**Important Note:**

* Use this script responsibly. Sending unsolicited LLDP packets could disrupt network operations.

**Features:**

* Creates LLDP PDUs with various TLVs (Type-Length-Value) including:
    * Chassis ID (randomly generated)
    * Port ID
    * Time to Live
    * Port Description
    * System Name (randomly generated)
    * System Description
    * System Capabilities
    * Management Address
    * Organization Specific TLV
* Allows customization of various LLDP parameters through configuration variables.

**Requirements:**

* Python 3
* Scapy library (install using `pip install scapy`)

**Usage:**

1. Install Scapy: `pip install scapy`
2. Modify the configuration variables in the script (`src_mac`, etc.) to suit your needs.
3. Run the script: `python lldp.py <number_of_LLDP_PDUs>` (replace `<number_of_LLDP_PDUs>` with the desired number of packets to send).

**Example:**

```bash
python lldp_generator.py 10
