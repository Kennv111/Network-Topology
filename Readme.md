# Bicol University - College of Science Network Topology

A comprehensive network design and simulation of the Bicol University College of Science (BUCS) campus, developed using **Cisco Packet Tracer**. This project simulates a robust, scalable, and secure campus network infrastructure tailored to the specific needs of the CS and Science departments.

## Project Overview
This project focuses on the architectural design of a functional network connecting the four primary buildings of the College of Science. It incorporates modern networking principles to ensure efficient data flow, security, and high availability for students and faculty.

## Campus Structure
The simulation includes dedicated network infrastructure for the following buildings:
* **CSB1:** Main Building 
* **CSB2:** CS/IT Building 
* **CSB3:** Biology/Chemistry Labs 
* **CSB4:** Meteorology / Lecture Rooms 

## Technical Specifications
The topology implements the following networking concepts and configurations:
* **VLAN Segmentation:** Logical grouping of departments to improve security and reduce broadcast traffic.
* **Inter-VLAN Routing:** Communication between buildings using Router-on-a-Stick or Layer 3 switching.
* **Dynamic Host Configuration Protocol (DHCP):** Automated IP address management for end devices in each building.
* **Domain Name System (DNS):** Internal resolution of hostnames for campus services.
* **OSPF Routing:** Implementation of **Open Shortest Path First** for dynamic, scalable routing between building clusters.
* **Port Security:** Layer 2 security measures to prevent unauthorized hardware from connecting to the network.

## The Team
This project was a collaborative effort by:
* **Kenneth B. Borjal**
* **Marx Ervic Delima**
* **Arbie Ancheta**
* **Sean Dylan Armenta**

## How to Run the Simulation
1.  **Software Requirement:** Ensure you have **Cisco Packet Tracer** (version 8.0 or higher) installed on your machine.
2.  **Download the Lab:** * Navigate to the `NETWOIpkt-1-1.pkt` file in this repository.
    * Click the **Download raw file** button to save the project to your local directory.
3.  **Open the Project:** Launch Cisco Packet Tracer and open the downloaded `.pkt` file.
4.  **Network Convergence:** Once the file opens, wait for approximately **30–60 seconds**. The link lights will initially appear red or amber; wait for them to turn **green** as the OSPF and Spanning Tree protocols initialize and establish neighbors.
5.  **Verifying Connectivity:**
    * **Simple PDU:** Select the **Envelope icon** (Simple PDU) from the right-side toolbar. Click on a PC in **CSB2** and then a PC in **CSB1**. The status should show **"Successful"** in the bottom-right panel.
    * **Command Line:** Select any end device (PC/Laptop), go to the **Desktop** tab > **Command Prompt**, and use the `ping` command to test communication between different building subnets (e.g., pinging from CSB3 to CSB4).

## License
This project was developed and submitted as a **Final Project for the course Networking 1** under the BS Information Technology curriculum at Bicol University. It is intended for academic and demonstration purposes only.
