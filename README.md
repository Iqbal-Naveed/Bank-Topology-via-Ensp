
# 🏦 Bank Network Topology via Huawei eNSP

A simulated enterprise-level **banking network topology** designed using **Huawei eNSP (Enterprise Network Simulation Platform)**. This project demonstrates real-world banking infrastructure concepts like **VLANs**, **Routing (Static & RIP)**, **Telnet**, **STP**, **ACLs**, **Eth-Trunk**, **DHCP**, and **FTP**, all through CLI-based implementation.

---

## 📌 Project Objective

To simulate a secure, scalable, and fully functional **bank network** with routers, switches, and hosts to:

* Ensure **segmented communication** between departments
* Enable **secure remote management**
* Implement **redundancy and load balancing**
* Provide **dynamic IP management** via DHCP
* Host FTP server for internal banking operations

---

## 🖥️ Tools Used

* **Huawei eNSP (Enterprise Network Simulation Platform)**
* **VRP CLI (Command Line Interface)**
* **Windows 10 as VM OS (for FTP Server)**
* **Wireshark (Optional) for packet analysis**

---

## 🗂️ Project Structure

```
Bank-Topology-via-Ensp/
├── Topology Screenshot.png       # Overview of the final topology
├── Configuration_Steps.pdf       # Step-by-step configuration guide
├── device-configs/               # Text files for router/switch CLI configs
│   ├── Router1.txt
│   ├── Switch1.txt
│   └── ...
├── ftp-server-config.docx        # Guide for setting up FTP in Windows VM
└── README.md                     # This file
```

---

## 🔧 Features Implemented

| Feature                          | Description                                                  |
| -------------------------------- | ------------------------------------------------------------ |
| **VLANs**                        | Logical segmentation by department (e.g., HR, Finance, IT)   |
| **Inter-VLAN Routing**           | Routers on a stick method for inter-department communication |
| **Static Routes**                | Manual path configuration between remote networks            |
| **RIP**                          | Dynamic routing for scalability                              |
| **Telnet Access**                | Remote CLI access via password-based login                   |
| **ACL (Access Control List)**    | Restrict unauthorized access to critical devices             |
| **STP (Spanning Tree Protocol)** | Avoid switch loop redundancy                                 |
| **Eth-Trunk (LACP)**             | Load balancing and redundancy via trunked ports              |
| **DHCP**                         | Dynamic IP assignment to end devices                         |
| **FTP Server**                   | Simulated secure file server using Windows VM                |

---

## 🚀 Getting Started

### 1. Setup Huawei eNSP

> Download from [Huawei eNSP Official Link](https://support.huawei.com/enterprise/en/network-management/ensp-pid-9017381)

### 2. Import the Topology

Manually replicate the provided topology based on the `Topology Screenshot.png` or `Configuration_Steps.pdf`.

### 3. Configure Devices

Use the `device-configs/` files and apply each CLI configuration manually to the respective devices:

```plaintext
[R1]interface g0/0/1
[R1-GigabitEthernet0/0/1]ip address 192.168.1.1 255.255.255.0
...
```

### 4. Setup FTP Server

Use `ftp-server-config.docx` to configure a basic Windows-based FTP server inside a VM connected to the network.

---

## 📸 Topology Preview

![Bank Network Topology](Topology%20Screenshot.png)

---

## 📚 Use Cases

* 🏛️ **Bank Branch Network Simulation**
* 🎓 **Academic Projects for Networking Students**
* 🔐 **ACL and Security Scenario Testing**
* 🧪 **Training Platform for Huawei Certifications**

---

## 📄 Requirements

* Huawei eNSP installed and running
* Sufficient CPU/RAM to run multiple virtual routers/switches
* Windows VM or alternative OS with FTP support

---

## 📌 Notes

* All IP addresses, VLAN IDs, and routing protocols are customizable.
* Use `save` or `save current configuration` after each device configuration.
* Telnet username and passwords must be set manually in router VTY lines.

---

## 🙌 Contributions

Pull requests are welcome! If you have enhancements (e.g., load balancing, firewall integration, SNMP monitoring), feel free to open an issue or PR.

---

## 📃 License

This project is open-sourced under the [MIT License](LICENSE).

---

## 👨‍💻 Author

Developed by **[Naveed Iqbal](https://github.com/Iqbal-Naveed)**
🎓 NEDUET University — Computer Science

---

