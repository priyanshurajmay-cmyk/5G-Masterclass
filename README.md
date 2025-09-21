# 5G-Masterclass

# 1. **Introduction to 5G**
* The next decade will be empowered by the capabilities of 5G technology.
* 5G enables three major categories of communication:
    1.  **Next-Level Wireless Broadband Experience:** Enhanced mobile broadband (eMBB).
    2.  **Massive Machine Type Communication (mMTC):** Allows for the deployment of a huge number of devices (e.g., IoT sensors).
    3.  **Ultra-Reliable Low-Latency Communication (URLLC):** Provides very high performance for critical applications (e.g., remote surgery, autonomous vehicles).

#### **Course Focus & Content**
* This course will explore the concepts that make up the **5G Radio Access Network (RAN)**.
* Key topics to be covered include:
    * Innovative features of 5G RAN.
    * Protocols used in the network.
    * Key procedures that make the network function.
* Understanding these functionalities is key to enabling the different use cases of 5G.

# 1.1 The 5G standardization

***

## 1. Introduction: The Need for Standardization

The development of a global technology like 5G raises two fundamental questions:
1.  **Who defines what 5G is?**
2.  **Who actually designs the technology for 5G?**

The process that answers these questions is **standardization**.

### The Power Outlet Analogy

<img width="1690" height="842" alt="image" src="https://github.com/user-attachments/assets/e7f7c937-b7a8-4f58-84d3-c5944518f398" />

To understand why a single global standard is crucial, consider the variety of electrical power outlets around the world. Over a century ago, as electricity was rolled out globally, different countries adopted different designs for their outlets for various reasons. This created several problems that a unified standard would have avoided:

* **Lack of Interoperability**: Travelers need multiple adapters because a plug from one country doesn't fit an outlet in another.
* **Higher Costs**: Manufacturing and maintaining many different designs is more expensive than producing a single, universal one.
* **Sub-optimal Design**: Instead of a single, superior design created through global collaboration, many different, potentially less efficient designs exist.

Telecommunications technology faces the same challenges. Without standardization, phones from one region wouldn't work in another, costs would be higher, and the technology would be less advanced.

***

## 2. The International Effort: ITU
<img width="1663" height="676" alt="image" src="https://github.com/user-attachments/assets/a31714da-39e4-40ca-8ca9-531a7d73dea6" />

The primary international body overseeing telecommunications is the **International Telecommunication Union (ITU)**, which is a specialized agency of the **United Nations**.

### History and Mission of the ITU

* **Establishment**: It was established as the International Telegraph Union way back in **1865**. Its name was later updated to reflect the evolution of technology.
* **Mission**: The ITU's mission is to "connect all the world's people."

The ITU is structured into three main sectors to manage its diverse responsibilities:

1.  **ITU-T (Telecommunication Standardization Sector)**: This group coordinates the creation of technical standards for information and communication technologies (ICTs). Its work covers areas like video compression, machine learning technologies, and cybersecurity.
2.  **ITU-R (Radiocommunication Sector)**: This is the most critical sector for wireless technology. It manages the global radio-frequency spectrum and satellite orbits, ensuring that wireless services can operate without interference. **ITU-R is directly involved in defining 5G**.
3.  **ITU-D (Telecommunication Development Sector)**: This group focuses on establishing policies, regulations, and providing training programs to help developing countries expand their access to ICTs.

***

## 3. Defining the 5G Requirements

<img width="2075" height="1127" alt="image" src="https://github.com/user-attachments/assets/713a1a42-d5a5-4490-9a8e-41ed63427d96" />

The ITU-R does not design the technology itself, but it **defines the requirements and capabilities** that a technology must meet to be officially called "5G."

* This process was done through a forum called **IMT-2020**, which was established in 2015.
* A similar forum, **IMT-Advanced**, was responsible for defining the requirements for 4G technology about a decade earlier.

The IMT-2020 forum produced a set of key performance indicators (KPIs) that 5G must achieve. These are often visualized in a "spider chart," comparing the goals for 5G (IMT-2020) with the capabilities of 4G (IMT-Advanced).

### The 8 Key Requirements of 5G


1.  **Peak Data Rate**: The maximum theoretical data rate a single user can achieve in perfect conditions.
    * **Target**: **20 Gbit/s**

2.  **User Experienced Data Rate**: The average speed a user should expect in real-world conditions with typical network load.
    * **Target**: **100 Mbit/s**

3.  **Spectrum Efficiency**: A measure of how efficiently the radio spectrum is used, indicating how many bits of data can be transmitted per hertz of frequency.
    * **Target**: **3x** improvement over 4G.

4.  **Mobility**: The maximum speed at which a user can travel while maintaining a seamless connection.
    * **Target**: Up to **500 km/h** (suitable for high-speed trains).

5.  **Latency**: The time delay for a packet of data to travel across the network.
    * **Target**: **1 millisecond (ms)**

6.  **Connection Density**: The number of connected devices that can be supported in a given area.
    * **Target**: **1 million ($10^6$) devices per square kilometer**.

7.  **Network Energy Efficiency**: The reduction in power consumption per bit of data transferred, crucial for device battery life.
    * **Target**: **100x** improvement over 4G.

8.  **Area Traffic Capacity**: The total amount of data traffic that can be supported per unit of area.
    * **Target**: **10 Mbit/s per square meter**.

***

## 4. Designing the Technology: 3GPP

<img width="1834" height="1107" alt="image" src="https://github.com/user-attachments/assets/9c44378d-7d23-4b5c-8448-9398b84d58c0" />

While the ITU defines *what* 5G should achieve, the **3rd Generation Partnership Project (3GPP)** is the organization that designs *how* to achieve it.

### What is 3GPP?

* **A Collaborative Effort**: 3GPP is a partnership of telecommunications standards organizations from across the globe (including Japan, China, South Korea, USA, Europe, and India).
* **Industry Participation**: It also includes a vast number of private companies, such as equipment vendors (Ericsson, Huawei), device manufacturers (Apple, Samsung), and chipset makers (Qualcomm, MediaTek).
* **Historical Context**: 3GPP is responsible for developing the world's most widely used mobile technologies, including:
    * **GSM** (2G)
    * **UMTS** (3G)
    * **LTE** (4G)
* **The "Other" 3GPP**: A competing organization, **3GPP2**, developed alternative technologies like CDMA2000 but 3GPP is the dominant standards body today.

### 3GPP Organizational Structure

<img width="1531" height="985" alt="image" src="https://github.com/user-attachments/assets/ace524c6-15be-4efe-a7cc-0cbeffaac9b6" />

3GPP is divided into three main **Technical Specification Groups (TSGs)**:

1.  **TSG RAN (Radio Access Network)**: Focuses on the "air interface" – the wireless connection between the device and the network. This includes radio layer specifications, protocol aspects, and performance requirements.
2.  **TSG CT (Core Network & Terminals)**: Deals with the core network architecture and the overall functionality of the end-user device (terminal).
3.  **TSG SA (Service & Systems Aspects)**: Manages the overall system architecture, service requirements, and security. It defines what services the network should provide, such as voice, video, and mission-critical applications.

***

## 5. Timelines and Releases

### ITU & 3GPP Collaboration Workflow

<img width="1529" height="869" alt="image" src="https://github.com/user-attachments/assets/00fd12d0-240a-4aa7-bad2-9a27f17f01ff" />

The development of 5G followed a clear, collaborative process between 2015 and 2020:

1.  **ITU defines requirements**: The ITU's IMT-2020 group published the list of requirements for 5G.
2.  **3GPP develops solutions**: 3GPP undertook extensive system design, technical studies, and evaluations to create a technology that meets those requirements.
3.  **3GPP submits technology**: 3GPP formally submitted its proposed 5G technology solution to the ITU.
4.  **ITU accepts and standardizes**: In **2020**, the ITU formally reviewed and accepted the 3GPP solution as the official global standard for 5G.

### 3GPP Releases Timeline

<img width="1932" height="996" alt="image" src="https://github.com/user-attachments/assets/b58a0bf5-9ef2-485f-b673-75e9eb8f358d" />

3GPP works in "Releases," which are updated sets of specifications published every 12 to 18 months. This allows for the continuous evolution of mobile technology.


* **3G**: Began with **Release 99** in 1999.
* **3.5G**: Technologies like HSDPA emerged from later releases.
* **4G (LTE)**: The first version was introduced in **Release 8** (2009).
* **4.5G (LTE-Advanced & LTE-A Pro)**: Enhancements introduced in subsequent releases.
* **5G**: The first official version was defined in **Release 15** (2019). It is continuously being improved in Releases 16, 17, and beyond.
* **5.5G**: A potential mid-cycle update, expected around 2024.
* **6G**: Following the roughly 10-year cycle, work on 6G is expected to formalize, with a potential release around 2029.

# 1.2 The 5G use cases

### The Three Dimensions of 5G Use Cases
5G technology is designed around three primary use cases that form a dimensional triangle. Understanding these use cases is crucial for designing the features required to serve them.

1. **Enhanced Mobile Broadband (eMBB)**

2. **Massive Machine Type Communications (mMTC)**

3. **Ultra-Reliable and Low Latency Communications (URLLC)**

<img width="1183" height="1036" alt="image" src="https://github.com/user-attachments/assets/f88e555f-5b07-4efc-ab84-751ef0c9bcfe" />

## 1. Enhanced Mobile Broadband (eMBB)
This use case is an evolution of the mobile broadband services common in 4G, designed to support more sophisticated and data-intensive applications, particularly advanced video streaming.

<img width="1820" height="1080" alt="image" src="https://github.com/user-attachments/assets/c7374f1a-71c2-4de1-bcb0-505c2278435c" />

## 2. Massive Machine Type Communications (mMTC)
This category focuses on connecting a very large number of devices that transmit small amounts of data infrequently, emphasizing long battery life and deep coverage.

<img width="1842" height="1019" alt="image" src="https://github.com/user-attachments/assets/2f5142f4-7174-4053-977f-e2df9751cd43" />

## 3. Ultra-Reliable and Low Latency Communications (URLLC)
URLLC is designed for mission-critical applications that demand extremely high reliability, availability, and very low latency.
<img width="1754" height="1051" alt="image" src="https://github.com/user-attachments/assets/0eae6a9d-787c-4646-827c-768f8b84be39" />


<img width="2107" height="1066" alt="image" src="https://github.com/user-attachments/assets/e38c6e50-9b4c-46f7-be1f-79083fd557e5" />


# 1.3 Overview of the 5G System Architecture

<img width="1683" height="719" alt="image" src="https://github.com/user-attachments/assets/507db158-43af-4eb6-9bab-df0fbb64c14d" />

At a high level, the 5G system connects User Equipment (UE) to an application server (e.g., Google) through several network domains. These domains are:
* **Access Network:** This is the 5G Radio Access Network (RAN), which uses "New Radio" (NR) technology to provide wireless connectivity to the UE.
* **Core Network:** This is the 5G Core Network (5GC), which is responsible for functions like mobility management, security, and subscription management.
* **Data Network:** This is the network that hosts the services the user wants to access, such as the internet.

### Key Architectural Principles

<img width="1461" height="836" alt="image" src="https://github.com/user-attachments/assets/255df9c8-ba29-4291-835f-a02b93414514" />

#### 1. Control and User Plane Separation
A fundamental principle of the 5G architecture is the separation of the Control Plane and the User Plane.
* **User Plane:** Transports the actual user data. This is shown in red in the diagrams.
* **Control Plane:** Carries the control and signaling information. This is shown in green in the diagrams.

<img width="1572" height="912" alt="image" src="https://github.com/user-attachments/assets/0c92fcc0-a84a-4ba4-b5e5-c874bb000699" />

This separation provides two main advantages:
* **Independent Scaling:** The network can be scaled differently based on user needs. For example, a network with many Massive MTC devices needs a larger control plane, while a network with mobile broadband users requires a larger user plane.
* **Flexible Deployment:** Network functions can be placed in different geographical locations to meet performance requirements, such as latency.

#### 2. Architecture Representations

<img width="1584" height="701" alt="image" src="https://github.com/user-attachments/assets/91bc0253-1900-40e2-8b7a-0db4ed449e88" />

The 5G system can be viewed in two ways:
* **Reference Point Representation:** The traditional method where explicitly labeled interfaces (like N1, N2, N3) connect different network functions.
* **Service-Based Representation:** A modern approach where core network functions are represented as microservices that communicate with each other. This course focuses on this representation.

### Key Network Functions

#### 5G RAN Components
* **gNodeB (gNB):** The 5G base station that uses New Radio (NR) technology. It is responsible for providing wireless connectivity to the UE.
* **Ng-eNB:** A base station that can support both NR and LTE.

#### 5G Core (5GC) Components
* **User Plane Function (UPF):**
    * Acts as the mobility anchor for the device as it moves.
    * Provides the interface to the external data network.
    * Enforces policies and is a point for lawful interception.
* **Session Management Function (SMF):**
    * Responsible for session management, such as establishing a new session and allocating an IP address to the device.
* **Access and Mobility Management Function (AMF):**
    * Manages device registration and mobility as it moves between radio cells.
    * Establishes the encrypted signaling connection with the UE.
* **Authentication Server Function (AUSF):**
    * Supports the AMF with authentication-related functions and security information.
* **Unified Data Management (UDM) / Unified Data Repository (UDR):**
    * The UDR stores all user subscription data.
    * The UDM is the front-end that manages this data, providing it to the AMF to assist with access authorization and registration.
* **Policy Control Function (PCF):**
    * Manages policies for session management and non-session management (like access control).
    * Supports charging-related functions based on device usage.

### Key Interfaces
The reference point architecture defines several key interfaces between network components:
* **N1:** Between the UE and the AMF.
* **N2:** The control plane interface between the gNodeB and the AMF.
* **N3:** The user plane interface between the gNodeB and the UPF.
* **N4:** The interface between the SMF and the UPF.

# 1.4 The 5G Deployment Options

### Introduction: Standalone vs. Non-Standalone

As mobile operators transition from 4G to 5G, they can't just flip a switch. For many years, 4G and 5G networks will coexist. This reality has led to two primary deployment strategies.

<img width="1549" height="893" alt="image" src="https://github.com/user-attachments/assets/2502bf01-de6f-458d-b993-a6aeba5d1eb3" />

* **Standalone (SA)**: A pure, end-to-end 5G network. This includes 5G base stations (**gNodeBs**) connecting to a **5G Core (5GC)** network. This is the ultimate goal for 5G, unlocking its full potential like ultra-low latency and network slicing.
* **Non-Standalone (NSA)**: A transitional approach where new 5G gNodeBs are added to an existing 4G network infrastructure. This allows operators to leverage their existing 4G Core network (**EPC**) and offer 5G speeds more quickly and economically.

Several specific deployment "Options" define how these components can be interconnected.

---

<img width="1672" height="901" alt="image" src="https://github.com/user-attachments/assets/6215bf31-4128-4544-82f8-6c98de1949c0" />

### Option 1: Legacy 4G LTE

This is the existing 4G network that serves as the baseline before any 5G deployment.

* **Radio**: 4G **eNodeB**.
* **Core**: 4G **EPC (Evolved Packet Core)**.
* This is a complete, self-contained 4G system.

---

### Option 2: 5G Standalone (SA)

This is the "true" 5G network, operating independently of any 4G infrastructure.


* **Radio**: 5G **gNodeB**.
* **Core**: **5G Core (5GC)**.
* **Characteristics**:
    * This is the target architecture for the full 5G experience.
    * It's required for advanced 5G use cases that depend on the new 5G core network's capabilities.
    * There is no interworking with a legacy 4G core network.

---

### Option 3: Non-Standalone (NSA) with EN-DC

<img width="1669" height="888" alt="image" src="https://github.com/user-attachments/assets/adb912b4-664a-4533-a4aa-73d8dd78b990" />

This is the most common initial deployment strategy for 5G, known as **EN-DC (E-UTRAN New Radio – Dual Connectivity)**.


* **Architecture**: The network uses both 4G eNodeBs and 5G gNodeBs, but everything connects to the existing **4G EPC**.
* **Control Plane (Signaling)**: The 4G **eNodeB** acts as the **master node**. It handles all the control signaling with the 4G core network. The green lines in the diagram show this control path.
* **User Plane (Data)**: The UE connects to both the 4G eNodeB and the 5G gNodeB. The **gNodeB** acts as a **secondary node** purely for a data speed boost. User data can be split and sent over both 4G and 5G paths simultaneously to increase throughput. The red lines in the diagram show the data path.
* **Why it's used**: It's a cost-effective way to launch 5G services quickly by reusing the existing 4G core and leveraging the wide coverage of the 4G network. It's ideal for areas with "spotty" initial 5G coverage.

#### Variants of Option 3

<img width="1664" height="923" alt="image" src="https://github.com/user-attachments/assets/15156ef1-b4f9-48aa-a581-47adc7ca6d36" />

There are slight variations of this option that define how the user data is split:
* **Option 3**: Data is sent from the core to the eNodeB, which then splits it between itself and the gNodeB.
* **Option 3a**: Data is split in the core network, with separate paths going to the eNodeB and gNodeB.
* **Option 3x**: A hybrid approach offering the most flexibility, where data can be split at either the eNodeB or the core network.

---

### Other Key Deployment Options

While Options 2 and 3 are the most prominent, other configurations exist for different migration scenarios.


* **Option 4 (NE-DC)**: This is the reverse of Option 3. It uses the **5G Core**, with the **gNodeB as the master node** for control signaling and the **eNodeB as a secondary data booster**. This becomes relevant when 5G coverage is mature and becomes the primary network.

<img width="1651" height="871" alt="image" src="https://github.com/user-attachments/assets/e91affd2-3e00-4d28-a55b-6917e1a703e3" />

  <img width="1674" height="1001" alt="image" src="https://github.com/user-attachments/assets/2672432c-c56b-42ef-91d3-592f94e07eac" />

* **Option 5**: An upgraded 4G base station, called an **eLTE eNodeB**, connects directly to the **5G Core**.

<img width="1255" height="956" alt="image" src="https://github.com/user-attachments/assets/bb4db2f3-5e05-4930-afa7-2c77240a15b7" />


* **Option 7**: A variation where an eLTE eNodeB connects to the **5G Core** and acts as the master node, with a gNodeB serving as the secondary node.

  <img width="1201" height="982" alt="image" src="https://github.com/user-attachments/assets/12f3effa-ef92-4987-b64c-225547eb0695" />

* **Option 6**: A configuration where a 5G gNodeB would connect to a 4G Core. This option is **not supported** by the standards.

<img width="1382" height="934" alt="image" src="https://github.com/user-attachments/assets/4c40aed6-397c-4563-9aed-8aac537ca313" />


# 2. 5G RAN Protocol Stack (2. 5G New Radio (NR) Radio Access Networks (RAN))

### The RAN Protocol Stack Overview

<img width="2093" height="1114" alt="image" src="https://github.com/user-attachments/assets/33f45844-75ad-4e58-85b8-933cbb7f82e9" />

The 5G New Radio (NR) system utilizes two distinct protocol stacks:

* **User Plane Protocol Stack**: This stack is responsible for carrying user data between applications on the User Equipment (UE) and the network.
* **Control Plane Protocol Stack**: This stack carries control information between the UE, the gNodeB (the 5G base station), and the core network.

In both stacks, each protocol layer communicates with its corresponding peer layer on the other end (e.g., the RLC layer on the UE communicates with the RLC layer on the gNodeB). Layers provide services to the layer above them and utilize services from the layer below.

---

### User Plane Protocol Stack

The User Plane stack handles all user data traffic. It consists of the following layers from top to bottom: SDAP, PDCP, RLC, MAC, and PHY.



#### **SDAP (Service Data Adaptation Protocol)**

<img width="1755" height="1092" alt="image" src="https://github.com/user-attachments/assets/9fe2f82e-eb95-40f3-aad4-535acddca24a" />

* **Primary Function**: Manages Quality of Service (QoS).
* **Details**: It maps QoS flows to specific data radio bearers to ensure that data from different applications (like video streaming vs. web browsing) receives the appropriate network treatment.

#### **PDCP (Packet Data Convergence Protocol)**

<img width="2012" height="1101" alt="image" src="https://github.com/user-attachments/assets/9c800bcb-cdc8-4c37-bfc9-461495822325" />

* **Primary Functions**: This layer adapts data for efficient and secure transmission over the radio interface.
* **Key Responsibilities**:
    * **Header compression** to reduce overhead.
    * **Ciphering & Integrity protection** for security.
    * **Duplicate removal** to handle retransmissions from lower layers.

#### **RLC (Radio Link Control)**

<img width="1818" height="1085" alt="image" src="https://github.com/user-attachments/assets/7ef87f3d-3179-48d9-bf4f-ca78321b9c69" />

* **Primary Functions**: Ensures reliable data transfer between the UE and gNodeB.
* **Key Responsibilities**:
    * **ARQ (Automatic Repeat Request)**: A robust error detection and retransmission scheme.
    * **Segmentation and Reassembly**: Breaks down larger packets into smaller units for transmission and puts them back together at the receiving end.

#### **MAC (Medium Access Control)**

<img width="1834" height="1081" alt="image" src="https://github.com/user-attachments/assets/444d4b1f-d011-4655-9eca-0bd09f2cf754" />


* **Primary Functions**: Manages access to the shared wireless channel.
* **Key Responsibilities**:
    * **Retransmission**: Handles very fast retransmissions using a process called Hybrid ARQ (HARQ).
    * **Multiplexing/Demultiplexing**: Combines data from different logical channels into single transport blocks.
    * **Scheduling**: Decides which users get to transmit and receive data at any given time.

#### **PHY (Physical Layer)**

<img width="2033" height="1114" alt="image" src="https://github.com/user-attachments/assets/cd5b4ee0-56ae-4b77-b84e-c66839d3aee5" />

* **Primary Function**: Responsible for the actual transmission and reception of bits and bytes over the air interface.
* **Details**: It handles efficient wireless communication through processes like channel coding, modulation, and managing multiple antennas.

---

<img width="1986" height="1113" alt="image" src="https://github.com/user-attachments/assets/3546b69d-08c4-43c4-bb08-cd24e004735a" />

### Control Plane Protocol Stack

The Control Plane stack manages the connection and radio resources. Its lower layers (PDCP, RLC, MAC, PHY) perform the same functions as in the User Plane. It includes two unique higher layers: RRC and NAS.



#### **NAS (Non-access Stratum)**

<img width="2004" height="1096" alt="image" src="https://github.com/user-attachments/assets/9198c63b-d5a1-45ab-965c-085bc41173c8" />

* **Communication**: Operates directly between the UE and the AMF (Access and Mobility Management Function) in the 5G core network. It is "non-access" because its messages are transparent to the gNodeB.
* **Key Responsibilities**:
    * Authentication and Security procedures.
    * Idle mode procedures, such as paging the UE when there is incoming data.
    * Establishing and managing communication sessions.

#### **RRC (Radio Resource Control)**

<img width="1947" height="1084" alt="image" src="https://github.com/user-attachments/assets/71c60538-5ad6-4d46-b6d4-4f52fa26ac66" />

* **Communication**: Operates between the UE and the gNodeB.
* **Key Responsibilities**:
    * Broadcasting System Information that UEs need to connect to the cell.
    * Setting up, modifying, and releasing Radio Bearers.
    * Managing UE measurement configuration and reporting for mobility (handovers).

---

### Key Concepts: SDU and PDU 

These terms describe how data is viewed at different layers of the protocol stack.

<img width="1965" height="998" alt="image" src="https://github.com/user-attachments/assets/e9b4f3ed-2aef-4673-9482-58f32e379165" />

* **SDU (Service Data Unit)**: The data packet that a layer receives from the layer directly above it. Think of it as the "cargo" that needs to be transported.
* **PDU (Protocol Data Unit)**: The data packet that a layer sends to the layer directly below it. It consists of the SDU (the cargo) plus a header added by the current layer for control purposes.

# 2.1 Service data Adaptation Protocol(SDAP)

***Service Data Adaptation Protocol (SDAP) and Quality of Service (QoS).***

### The Need for QoS in 5G

5G is designed to support a wide variety of services with very different network requirements. This diversity makes a "one-size-fits-all" approach to data handling impossible.

<img width="1666" height="917" alt="image" src="https://github.com/user-attachments/assets/05820854-334d-4fa7-b27b-114466500fea" />

* **Voice**: Requires a steady, continuous flow of data, but at a low data rate.
* **Broadband**: Involves bursty traffic with very high data rates, like web browsing or file downloads.
* **Massive MTC (Machine-Type Communications)**: Characterized by a huge number of devices sending small amounts of data infrequently.
* **URLLC (Ultra-Reliable Low-Latency Communications)**: Demands extremely high reliability and very low delay, crucial for applications like remote surgery or autonomous vehicles.

To handle this, 5G uses a **Quality of Service (QoS)** framework. QoS is the mechanism that manages data traffic to ensure each application gets the performance it needs by prioritizing different data flows.

---

### Understanding QoS Flows

<img width="1708" height="910" alt="image" src="https://github.com/user-attachments/assets/23f1839d-4f6c-46dc-b052-433fe5029586" />

The foundation of 5G QoS is the **QoS Flow**.

A QoS Flow is the finest level of granularity for policy enforcement and data handling. Think of it as a dedicated "pipe" for a specific type of data traffic from the User Equipment (UE) all the way to the UPF (User Plane Function) in the core network, which connects to the internet.


* Each packet belonging to a specific application or service is mapped to a QoS Flow.
* Every QoS Flow is identified by a **QoS Flow Identifier (QFI)**.
* Packets with the same QFI receive the same traffic treatment (e.g., same priority, latency, and reliability).

---

### Types of QoS Flows

There are three main types of QoS flows, each defined by the guarantees it provides.

<img width="1659" height="724" alt="image" src="https://github.com/user-attachments/assets/3897b565-dcea-45ab-9eba-35b3c8ace162" />

* **GBR (Guaranteed Bit Rate)**: This flow type is for services that need a reserved, constant data rate. It's essential for applications that can't tolerate interruptions.
    * **Example**: Conversational voice calls or live video streaming.
* **Non-GBR (Non-Guaranteed Bit Rate)**: This is a "best effort" flow. The network doesn't reserve a specific data rate, making it suitable for applications that can handle variations in speed and are bursty in nature.
    * **Example**: Web browsing, email, and file downloads.
* **Delay-Critical GBR**: A specialized GBR flow for URLLC services that require both a guaranteed data rate and extremely low latency.
    * **Example**: Remote control of machinery or vehicle-to-everything (V2X) communications.

<img width="1676" height="889" alt="image" src="https://github.com/user-attachments/assets/32cdc977-25cb-4932-b075-e3b48b271b68" />

<img width="1590" height="979" alt="image" src="https://github.com/user-attachments/assets/706686b7-7b9e-4260-869d-4f8f8217360b" />

---

### The Role of the SDAP Layer 

<img width="1640" height="962" alt="image" src="https://github.com/user-attachments/assets/08beaff5-4d72-4636-982c-cb0e3520175c" />

The **Service Data Adaptation Protocol (SDAP)** is a protocol layer in the 5G Radio Access Network (RAN) whose primary job is to manage QoS.

The core network deals with QoS in terms of **QoS Flows**. The radio network, however, transports data over **Radio Bearers**. The key function of the SDAP layer is to be the bridge between these two concepts.

**SDAP maps the QoS Flows from the core network to the appropriate Data Radio Bearers (DRBs) for transmission over the air.**

<img width="1630" height="938" alt="image" src="https://github.com/user-attachments/assets/9b42ea6c-cb23-4262-b044-29cd5e73b959" />

For example, multiple Non-GBR QoS flows (like web browsing, WhatsApp messages, and a YouTube video) might be mapped by the SDAP layer onto a single "best effort" Radio Bearer. At the same time, a high-priority GBR flow (like a Zoom video call) might be mapped to its own dedicated Radio Bearer to guarantee its performance.

### Uplink QoS Mapping

<img width="1671" height="716" alt="image" src="https://github.com/user-attachments/assets/c5dc28d4-499a-48dd-b5b1-1e0682cd96bd" />

For uplink traffic (from the UE to the network), there are two ways to map data to the correct QoS flow:

* **Reflective Mapping**: The UE automatically mirrors the mapping used in the downlink. If it receives data for a specific service on a certain QoS Flow, it will use that same flow for sending data for that service.
* **Explicit Mapping**: The network uses RRC (Radio Resource Control) signaling to explicitly tell the UE which QoS Flow to use for its uplink traffic.

# 2.2 Packet data convergence protocol (PDCP)

### Introduction to PDCP

The **Packet Data Convergence Protocol (PDCP)** is a key layer in the 5G protocol stack, sitting just below the SDAP layer. Its primary role is to process IP packets to make them suitable for efficient and secure transmission over the radio interface.

<img width="1102" height="677" alt="image" src="https://github.com/user-attachments/assets/3e0a1171-ff9c-4153-90c9-bf294b3cf6aa" />

The main functions of PDCP include:
* Header Compression
* Ciphering and Integrity Protection (Security)
* Routing and Duplication for Split Bearers
* In-sequence delivery of data

---

### Header Compression 

IP packets have large headers (**40 bytes for IPv4, 60 bytes for IPv6**). For applications that send small amounts of data, like voice calls, this header is a significant overhead.

<img width="1505" height="853" alt="image" src="https://github.com/user-attachments/assets/b1a208aa-f607-48b0-93e8-c139cae6eef4" />

PDCP solves this using **Robust Header Compression (ROHC)**. This technique compresses the large IP/UDP/RTP headers down to just a few bytes, freeing up valuable space on the radio interface for actual user data. The PDCP layer on the receiving end is then responsible for decompressing the header back to its original format.


---

### Ciphering & Integrity Protection 

PDCP is responsible for securing the data transmitted over the air. It provides two main security functions:

<img width="1647" height="753" alt="image" src="https://github.com/user-attachments/assets/b3543190-5c2d-4ecf-89af-ef95f6bd4aa5" />

* **Ciphering (Confidentiality)**: This process encrypts the user data to prevent eavesdropping. It uses an **Encryption Algorithm (NEA)** along with a security key to convert the plaintext data into ciphertext before transmission. The receiver uses the same key and algorithm to decrypt the data.
* **Integrity Protection (Authenticity)**: This ensures that the data has not been altered in transit and originates from a trusted source. It uses an **Integrity Algorithm (NIA)** to create a Message Authentication Code (MAC) that is appended to the message. The receiver recalculates this code and verifies it to ensure the message's integrity.


---

### Routing & Duplication (Split Bearer) 

5G supports **Dual Connectivity**, where a device can be connected to two cell towers simultaneously: a **Master Cell** and a **Secondary Cell**. PDCP manages the data flow in this scenario.

<img width="1662" height="859" alt="image" src="https://github.com/user-attachments/assets/e1d9ec9c-0bae-453e-aad5-15e95ff4f4e5" />

* **Routing (Split Bearer)**: To increase the data rate, PDCP can split a single data stream (a bearer) across both the Master and Secondary cells. This allows the device to aggregate the bandwidth from both cells.
* **Duplication**: To increase reliability, PDCP can duplicate data packets and send identical copies over both the Master and Secondary cell paths. The receiving PDCP layer is then responsible for discarding any duplicate packets that arrive, ensuring the higher layers only receive one copy. This is critical for ultra-reliable services.

---

### In-sequence Delivery 

Some applications require that data packets are received in the exact order they were sent, while others do not. PDCP can handle both scenarios.

<img width="1651" height="831" alt="image" src="https://github.com/user-attachments/assets/ce819c68-6f7f-4c96-925f-8867e9b44f3d" />

* **Out-of-sequence delivery**: Packets are sent to the higher layers as soon as they arrive from the radio link, even if they are out of order. This is suitable for services like file transfers where the higher-level TCP protocol can handle reordering.
* **In-sequence delivery**: PDCP adds a **Sequence Number** to each packet. On the receiving side, it uses a buffer to reorder any packets that arrive out of sequence before delivering them to the higher layers. This is essential for real-time applications like video streaming to avoid glitches.

<img width="1459" height="972" alt="image" src="https://github.com/user-attachments/assets/f11e192e-adf1-4f24-b540-01af802944ed" />

# 2.3 Radio Link Control (RLC)

The Radio Link Control (RLC) layer is a part of the 5G NR protocol stack that sits between the Packet Data Convergence Protocol (PDCP) layer and the Medium Access Control (MAC) layer.

### Main Functions of RLC

The RLC layer has two primary functions:

<img width="683" height="386" alt="image" src="https://github.com/user-attachments/assets/8619b777-bf79-4dac-a8fe-2f763f5d1430" />

* **Segmentation**: Breaking down or combining data packets to fit the transport block size provided by the lower physical layer.
* **ARQ (Automatic Repeat Request)**: Handling retransmissions of lost data packets to ensure reliable data delivery.

---

### RLC Modes

To cater to the different requirements of various applications, the RLC can operate in one of three modes.

<img width="1512" height="896" alt="image" src="https://github.com/user-attachments/assets/1ac6e8cb-aac4-487f-98dc-8876bf409b79" />

1.  **Transparent Mode (TM)**
    * In this mode, the RLC layer is essentially bypassed and does not perform any of its main functions.
    * **Features**:
        * No retransmission.
        * No duplicate detection.
        * No segmentation or reassembly.
    * **Use Case**: Primarily used for broadcasting control plane information on channels like BCCH, CCCH, and PCCH, where segmentation and retransmissions are unnecessary.

2.  **Unacknowledged Mode (UM)**
    * This mode provides segmentation services but does not offer guaranteed delivery through retransmissions.
    * **Features**:
        * Performs segmentation and reassembly.
        * Does not perform retransmissions.
    * **Use Case**: Suitable for services where low latency is critical and some data loss is acceptable, such as Voice over IP (VoIP).

3.  **Acknowledged Mode (AM)**
    * This is the most comprehensive mode, providing reliable data transfer using both segmentation and retransmissions.
    * **Features**:
        * Handles retransmissions.
        * Performs segmentation and reassembly.
        * Provides duplicate removal.
    * **Use Case**: Essential for services that require error-free data delivery, such as web browsing and file transfers.

---

### Segmentation

<img width="1427" height="908" alt="image" src="https://github.com/user-attachments/assets/59c07cee-cdcd-41a2-b36e-f4867e111224" />

Segmentation is the process where the RLC layer adapts the size of upper layer data packets, known as RLC Service Data Units (SDUs), to fit into the transport blocks for transmission by the MAC layer. The resulting packets are called RLC Protocol Data Units (PDUs).

The RLC PDU header contains several key fields to manage this process:
* **SDU Sequence Number (SN)**: A unique number assigned to each RLC SDU to track packets. The size of the sequence number can be 6/12 bits in UM and 12/18 bits in AM.
* **Segmentation Information (SI)**: This field indicates whether a PDU contains a complete SDU, or if it is the first, middle, or last segment of an SDU.
* **Segmentation Offset (SO)**: For segmented PDUs, this field specifies the starting point of the segment within the original SDU, which is crucial for correct reassembly at the receiver.

#### RLC Concatenation in NR vs. LTE

* In **LTE**, multiple RLC PDUs were often concatenated by the RLC layer itself into a single, larger PDU before being passed to the MAC layer.
* In **5G NR**, this concatenation function is moved from the RLC layer to the MAC layer. This change reduces latency, as the RLC layer can prepare PDUs immediately without waiting for a scheduling grant from the base station to know the final transport block size.

---

### Retransmissions (ARQ)

<img width="825" height="723" alt="image" src="https://github.com/user-attachments/assets/05c666c8-57a0-4893-a195-f350e30f55c7" />

The ARQ function in RLC Acknowledged Mode ensures reliable data delivery by retransmitting lost PDUs.

#### In-Sequence Delivery in NR vs. LTE

A significant change in 5G NR is that the RLC layer is no longer responsible for ensuring in-sequence delivery of packets to the upper layers. In LTE, RLC had to reorder packets and wait for any missing ones before delivering them. In NR, this function is optionally handled by the PDCP layer.

This change provides two main benefits:
1.  **Lower Latency**: Packets that arrive out of order can be delivered immediately to the PDCP layer without waiting for the retransmission of a missing packet, which is critical for low-latency applications.
2.  **Reduced Buffering**: Since the RLC layer doesn't need to buffer subsequent packets while waiting for a missing one, memory requirements are reduced.

#### Retransmission Process Example

The retransmission process involves coordination between the transmitter and receiver using transmit/receive windows and status reports.

1.  **Initial Transmission (T0)**: The transmitter sends PDUs. PDUs that have been successfully received and acknowledged are marked (e.g., in green). Those transmitted but not yet acknowledged are kept in the transmit buffer (e.g., in red). The transmit window starts from the first unacknowledged PDU.

2.  **Packet Loss (T1)**: The transmitter sends PDUs `n+1` and `n+2`, but the receiver only gets `n+2`. The receiver notes the gap and starts a **reassembly timer**, but immediately forwards the received `n+2` PDU to the upper layers.

3.  **Missing Packet Arrives (T2)**: If the missing PDU (`n+1`) arrives before the timer expires, the timer is stopped, and the packet is processed.

4.  **Timer Expiry and Status Report (T3-T4)**: If transmission continues and more packets are lost (e.g., `n+3` and `n+4`), the receiver's reassembly timer will eventually expire. Upon expiry, the receiver sends a **Status Report** back to the transmitter, indicating which PDUs are missing.

5.  **Retransmission (T5)**: Upon receiving the Status Report, the transmitter retransmits only the missing PDUs (`n+3` and `n+4`). It also advances its transmission window, as the report implicitly acknowledges all PDUs up to the first missing one.

6.  **Successful Reception (T6)**: Once all PDUs, including the retransmitted ones, are successfully received, the transmission is complete. The transmitter can request a final status report to confirm the delivery of all data.

# 2.4 Medium Access Control (MAC) Layer


## 5G NR: Medium Access Control (MAC) Layer

The Medium Access Control (MAC) layer sits between the RLC and Physical (PHY) layers in the 5G protocol stack. It manages how and when data is transmitted over the air interface.

---

### Functions of the MAC Layer

The MAC layer is responsible for several key functions in the 5G air interface:

* **Logical Channel Multiplexing**: It combines data from various logical channels into a single data stream for transmission.
* **Hybrid ARQ (HARQ) Retransmissions**: It manages a rapid retransmission protocol to correct errors that occur during transmission.
* **Scheduling**: It determines which users get to transmit or receive data at any given time, managing the allocation of radio resources.
* **Multiplexing for Carrier Aggregation (CA)**: When multiple carriers are used simultaneously, the MAC layer distributes the data across them.

---

### Multiplexing and Channel Mapping

The MAC layer acts as a bridge between two types of channels:

<img width="1581" height="815" alt="image" src="https://github.com/user-attachments/assets/2b958c4f-9eca-48df-8bcb-5bf05210fdf5" />

* **Logical Channels**: These channels are defined by the **type of information** they carry. They are the interface to the RLC layer above. Examples include:
    * **PCCH** (Paging Control Channel)
    * **BCCH** (Broadcast Control Channel)
    * **CCCH** (Common Control Channel)
    * **DCCH** (Dedicated Control Channel)
    * **DTCH** (Dedicated Traffic Channel)

<img width="1465" height="858" alt="image" src="https://github.com/user-attachments/assets/571fe3f4-eb7a-483b-b2f3-eb52b57afa75" />

* **Transport Channels**: These channels define **how data is transmitted** over the air interface, including its characteristics. They are the interface to the PHY layer below. Examples include:
    * **PCH** (Paging Channel)
    * **BCH** (Broadcast Channel)
    * **DL-SCH** (Downlink Shared Channel)
    * **UL-SCH** (Uplink Shared Channel)

The core multiplexing function of the MAC layer is to map the data from the various logical channels onto the appropriate transport channels for transmission.


---

### MAC Control Elements (CEs)

In addition to user data from the RLC layer, the MAC layer can insert its own control information directly into the data packets (MAC PDUs). These pieces of control information are known as **MAC Control Elements (CEs)**.

<img width="1366" height="738" alt="image" src="https://github.com/user-attachments/assets/56fb32e5-de39-41f5-9412-37367d7e271e" />

This is a form of in-band signaling used to manage various radio link functions, such as:
* Scheduling requests
* Timing advance commands
* Random access procedures

A complete MAC PDU is constructed from multiple components, including a header, MAC SDUs (the data payload from RLC), one or more MAC CEs, and padding to fill the transport block if necessary.

---

<img width="1001" height="778" alt="image" src="https://github.com/user-attachments/assets/4b2f93c7-b238-4831-af44-758c3825af00" />

### Hybrid ARQ (HARQ)

<img width="1180" height="841" alt="image" src="https://github.com/user-attachments/assets/9f4da7ad-aac6-48d5-99da-abcfb9ccf8cd" />

HARQ is a critical function for ensuring fast and reliable data transmission. It's called "hybrid" because it combines high-speed retransmissions (managed by MAC) with error correction coding (performed by the PHY layer).

#### Stop-and-Wait Protocol

<img width="1502" height="893" alt="image" src="https://github.com/user-attachments/assets/7ea7077a-f06e-408a-8fa6-edf91628fcb1" />

The fundamental HARQ mechanism is a **stop-and-wait** protocol. A transmitter sends a data block and then waits for feedback from the receiver:
* If the block is received correctly, the receiver sends an **ACK (Acknowledgement)**.
* If the block has errors, the receiver sends a **NAK (Negative Acknowledgement)**, and the transmitter resends the block.

While simple, waiting for feedback for every single packet is inefficient and introduces latency.

#### Parallel HARQ Processes

To overcome the inefficiency of a single stop-and-wait process, 5G NR runs **multiple HARQ processes in parallel**. This allows the transmitter to send new data blocks using other available processes while one process is waiting for an ACK/NAK. This pipelined approach significantly increases throughput and efficiency.


#### Asynchronous HARQ

A key difference from LTE is that 5G NR uses **asynchronous HARQ**.
* In LTE's **synchronous** system, the timing for HARQ feedback was fixed and predictable.
* In NR's **asynchronous** system, the feedback timing is flexible. The specific HARQ process the feedback belongs to is explicitly indicated in the Downlink Control Information (DCI). This flexibility is essential to support dynamic TDD configurations and advanced scheduling in 5G.

---

### Code Block Group (CBG) Retransmissions

5G allows for very large transport blocks. If a single bit error occurs in a large block, retransmitting the entire block is highly inefficient. To solve this, **Code Block Group (CBG)-based retransmission** is used.

<img width="1188" height="534" alt="image" src="https://github.com/user-attachments/assets/8a0b3250-309c-44c1-96ad-6cddaa942278" />

1.  A large Transport Block is first segmented into smaller **Code Blocks (CBs)** at the physical layer.
2.  These CBs are then bundled into **Code Block Groups (CBGs)**.
3.  When a transmission error occurs, the receiver's HARQ feedback can pinpoint exactly which **CBG** failed, rather than just marking the entire transport block as failed.
4.  The transmitter then only needs to re-send the specific CBG that contained the error, saving significant radio resources and improving efficiency.

<img width="1379" height="775" alt="image" src="https://github.com/user-attachments/assets/556ebbe8-2cfd-4ab8-a27e-b44626c03101" />

# 2.5 MAC Scheduler

## 5G NR: The MAC Scheduler

The scheduler is one of the most critical components in a 5G base station (gNodeB). It's the intelligent process that manages and allocates the network's finite radio resources among all the different users in a cell.

---

### What is a Scheduler?

<img width="1531" height="861" alt="image" src="https://github.com/user-attachments/assets/dfbed7ca-ebf1-4406-8919-e491f67e5763" />

At its core, the scheduler's job is to manage **shared channel transmission**. The radio resources, which are composed of time and frequency blocks, are a shared pool. The scheduler dynamically decides which user gets to use which specific time-frequency blocks for either sending (uplink) or receiving (downlink) data.

This decision-making process is continuous, happening on a very short timescale (every slot) to adapt to the constantly changing needs of the users and the radio environment.


---

### The Scheduler's Role and Inputs

<img width="1337" height="886" alt="image" src="https://github.com/user-attachments/assets/3fcde896-1c4f-4866-8824-d4475200b319" />

Although the scheduler is officially part of the MAC layer, it acts as a central control unit that interacts with multiple layers. To make intelligent decisions, the scheduler relies on several key inputs:

* **Channel Conditions**: Information about the quality of the radio link for each user. This is gathered from measurements of reference signals (like CSI-RS and SSB) and reported back by the device.
* **Buffer Status**: Reports indicating how much data each user has waiting in their queue to be sent or received.
* **Data Flow Priority**: Information about the Quality of Service (QoS) requirements for each data flow, such as whether it's for a low-latency application or a best-effort file transfer.

Based on these inputs, the scheduler's main **outputs** or decisions are:
* Which **devices** to schedule.
* Which **resource blocks** to assign to each device.
* The **transport format** to use, which includes the modulation scheme, coding rate, transport block size (TBS), and antenna configuration.

---

### Downlink Scheduling

<img width="1465" height="868" alt="image" src="https://github.com/user-attachments/assets/71079207-fb65-46b3-9125-c5abccc38124" />

In downlink scheduling, the gNodeB's scheduler determines how data is sent to the user devices (UEs).

<img width="1278" height="862" alt="image" src="https://github.com/user-attachments/assets/a6b096dd-f1d2-46d8-824d-d5b521b4bb69" />

#### Channel-Dependent Scheduling

The scheduler leverages a powerful concept called **multi-user diversity**. Since different users experience different channel conditions across the frequency band at any given moment, the scheduler can achieve significant efficiency gains by assigning frequency blocks to the users who have the best signal quality on those specific blocks at that instant.

#### Bandwidth Parts (BWP)

<img width="1265" height="840" alt="image" src="https://github.com/user-attachments/assets/7448eb12-b6c8-4818-88a2-2820a0b2539b" />

To save battery on mobile devices, a UE doesn't have to monitor the entire, very wide 5G carrier bandwidth all the time. Instead, it can operate on a smaller, configurable portion of the bandwidth called a **Bandwidth Part (BWP)**. The scheduler can dynamically adapt the UE's active BWP:
* **Narrow BWP**: Used for idle periods or low-data activity to conserve power.
* **Wide BWP**: The scheduler can instruct the UE to switch to a wider BWP when a large amount of data needs to be transferred quickly.

#### Preemption

<img width="1455" height="879" alt="image" src="https://github.com/user-attachments/assets/bcc47e14-cf2c-411b-96a6-8953259c71da" />

To support ultra-low latency services, 5G allows for **preemption**. If a low-priority, high-data-rate transmission is in progress, a new, high-priority, low-latency packet can interrupt (or preempt) it. The scheduler sends a "preemption indicator" to the first device, telling it to discard the data from the preempted resources. This ensures that critical data is sent immediately, without waiting for the ongoing transmission to finish.

#### Scheduling Types

* **Dynamic Scheduling**: This is the default mode. For every transmission, the gNodeB sends a **Downlink Control Information (DCI)** message to the UE, providing a specific grant of resources for that single transmission.
* **Configured Scheduling (Semi-Persistent Scheduling - SPS)**: This is ideal for predictable, periodic traffic like VoIP. The gNodeB pre-configures a recurring set of resources for the UE. The UE can then receive data on these resources without needing a DCI each time. A DCI can be sent to activate or deactivate this periodic grant or to override a specific transmission if needed.

---

### Uplink Scheduling

In uplink scheduling, the gNodeB's scheduler controls when and how the UEs transmit data to the network.

<img width="1521" height="881" alt="image" src="https://github.com/user-attachments/assets/c7bfacd1-6f7c-408b-88be-b94eaf7e3ebf" />

#### The Uplink Scheduling Process

<img width="1497" height="818" alt="image" src="https://github.com/user-attachments/assets/d256dcd9-181e-4e26-b0d1-f7704daed56f" />

The scheduler in the gNodeB makes decisions based on:
* **Uplink Channel Quality**: This is estimated by the gNodeB based on **Sounding Reference Signals (SRS)** that the UE is configured to transmit.
* **Buffer Status**: The UE sends reports to the gNodeB indicating how much data it has waiting to send.

Based on this information, the gNodeB sends an **uplink grant** (via DCI) to the UE, telling it exactly which time-frequency resources it is allowed to use for its transmission.

#### Key Differences from Downlink Scheduling

* Uplink transmissions are typically **power-limited**, not bandwidth-limited. A UE's maximum transmission power is a key constraint.
* Scheduling is **per-device**. The gNodeB grants a chunk of resources to a device, but the UE's internal logic decides which of its data flows (e.g., from different apps) gets priority to be sent using that grant.

#### Uplink Scheduling Types

Similar to the downlink, the uplink supports both **Dynamic Scheduling** and two types of **Configured Scheduling**:
* **Type 1 (Grant-Free)**: The UE is given a pre-configured, periodic resource and can transmit without receiving a specific DCI grant. This is useful for reducing latency for periodic data.
* **Type 2 (Configured Grant)**: The resources are pre-configured, but a DCI from the gNodeB is required to activate them for transmission.

# 2.6 Physical Layer(PHY)

The Physical Layer (PHY) is the lowest layer in the 5G protocol stack, sitting just below the MAC layer. It is responsible for the actual transmission and reception of data over the radio interface.

---

### Physical Channels vs. Transport Channels

The physical layer receives data from the MAC layer through **transport channels** and maps this data onto **physical channels**.

<img width="1551" height="666" alt="image" src="https://github.com/user-attachments/assets/d3140973-5ec2-4b6a-9d56-eb73232813d2" />

* **Transport Channels** (e.g., PCH, BCH, DL-SCH, UL-SCH) are defined by how data is transported.
* **Physical Channels** are defined by the specific set of time-frequency resources used for transmission.

The main physical channels in 5G NR are:

<img width="1534" height="898" alt="image" src="https://github.com/user-attachments/assets/b8fa9051-9749-4ad7-901c-1a83c7322a0c" />

#### Downlink Channels:
* **PBCH (Physical Broadcast Channel)**: Carries essential system information.
* **PDSCH (Physical Downlink Shared Channel)**: The main channel for user data and other control information.
* **PDCCH (Physical Downlink Control Channel)**: Carries scheduling information and other control commands.

#### Uplink Channels:
* **PUSCH (Physical Uplink Shared Channel)**: The main channel for user data transmitted from the device to the network.
* **PUCCH (Physical Uplink Control Channel)**: Carries control information from the device, such as HARQ acknowledgements.
* **PRACH (Physical Random Access Channel)**: Used for the initial random access procedure when a device wants to connect to the network.

---

### Downlink Shared Channel (DL-SCH) Processing

The journey of data from the MAC layer through the physical layer for a downlink transmission involves several key steps to prepare it for the air interface:

<img width="1273" height="808" alt="image" src="https://github.com/user-attachments/assets/c2cc0824-e06d-4697-8fe9-9302ebc4e10d" />

1.  **CRC Attachment**: A **Cyclic Redundancy Check (CRC)** is added to the transport block. This is an error detection code that allows the receiver to verify if the entire block was received correctly.

<img width="1627" height="747" alt="image" src="https://github.com/user-attachments/assets/805ce3f3-2e4e-4e6a-816c-23d2b8d7ac1f" />

2.  **Code Block Segmentation**: If a transport block is very large, it's broken down into smaller segments called **Code Blocks (CBs)**. A CRC is also added to each individual code block. This is crucial for efficient retransmissions, as only the erroneous code blocks need to be resent, not the entire transport block.

<img width="1600" height="753" alt="image" src="https://github.com/user-attachments/assets/c6450e0d-2533-410c-8a5d-b63f916016d5" />

3.  **LDPC Coding**: **Low-Density Parity-Check (LDPC)** coding is the primary error correction technique used in 5G for data channels. It adds redundant bits to the data, which helps the receiver to correct errors that occur during transmission over the noisy radio channel. 5G NR uses two different LDPC "base graphs" (BG1 and BG2) depending on the transport block size and the coding rate to optimize performance.

<img width="1642" height="862" alt="image" src="https://github.com/user-attachments/assets/6095d5d5-739f-47c5-b4cd-6d5eb8f41540" />

4.  **Rate Matching**: This step selects the exact number of bits that will be transmitted in a given time slot. It ensures that the amount of data perfectly matches the allocated radio resources.

<img width="1636" height="794" alt="image" src="https://github.com/user-attachments/assets/435d173e-604a-45dc-a73e-4faa49d21b08" />

5.  **Scrambling**: The data is multiplied by a cell-specific scrambling sequence. This makes the signal appear like random noise to devices in neighboring cells, which helps to reduce inter-cell interference.

<img width="1639" height="870" alt="image" src="https://github.com/user-attachments/assets/4fbe08ff-2a48-49c2-8d86-8a3df879895d" />

6.  **Modulation**: The scrambled bits are mapped to complex-valued modulation symbols. 5G NR supports several modulation schemes, including **QPSK, 16QAM, 64QAM, and 256QAM**, for both uplink and downlink. Higher-order modulation schemes can carry more data but require better signal quality.

<img width="1576" height="933" alt="image" src="https://github.com/user-attachments/assets/5e10a924-ad3a-45ad-a0db-76825ed52307" />

7.  **Layer Mapping**: The modulation symbols are mapped onto one or more transmission layers. This is part of the MIMO (Multiple-Input Multiple-Output) technology, where multiple data streams can be sent simultaneously to increase data rates.

<img width="1587" height="764" alt="image" src="https://github.com/user-attachments/assets/73b1a8ac-97e3-47b5-a77d-5bb4cc64c34c" />

9.  **Precoding**: This is another MIMO technique where the data layers are multiplied by a precoding matrix. This process "shapes" the signal to align with the specific characteristics of the radio channel, which helps to improve the signal quality at the receiver. This step maps the data layers to virtual antenna ports.

<img width="1603" height="847" alt="image" src="https://github.com/user-attachments/assets/42f3324a-12ee-4301-8793-df0e4a9cecea" />

10.  **Resource Mapping**: The precoded symbols for each virtual antenna port are mapped to the specific time-frequency resource elements that have been allocated by the scheduler for this transmission.

<img width="1537" height="813" alt="image" src="https://github.com/user-attachments/assets/5dfc2b1a-11be-4b92-83ff-d620b1324651" />

11. **OFDM Signal Generation**: Finally, an **Orthogonal Frequency-Division Multiplexing (OFDM)** signal is generated for each antenna port. This involves an Inverse Fast Fourier Transform (IFFT) and digital-to-analog conversion before the signal is sent to the RF (Radio Frequency) unit for transmission.

<img width="1431" height="815" alt="image" src="https://github.com/user-attachments/assets/382695c1-2be4-4f7e-8c3d-413bb2a65ad6" />

# 2.7 Physical Layer Structure

## 5G NR: Physical Layer Structure

The physical layer in 5G New Radio (NR) is designed with immense flexibility to handle a wide variety of services, from high-speed mobile broadband to ultra-reliable low-latency communications. This is achieved through a versatile structure encompassing its modulation scheme, multiple access techniques, and a flexible time-domain organization.

---

### Modulation Scheme: OFDM and its Variants

<img width="1618" height="874" alt="image" src="https://github.com/user-attachments/assets/0cf0506c-2b09-4051-bec7-0a1f4afa1975" />

Orthogonal Frequency-Division Multiplexing (OFDM) is the core modulation scheme for 5G NR. It's a technique that transmits a wideband signal by breaking it down into multiple narrowband signals, each carried on an orthogonal subcarrier. This approach is highly effective at combating frequency-selective fading, a common problem in wireless channels where certain frequencies are attenuated more than others.

<img width="1610" height="842" alt="image" src="https://github.com/user-attachments/assets/ba8f4790-1c80-49a4-a6e4-a2a9c434dd23" />

To further mitigate inter-symbol interference caused by multipath propagation, a **Cyclic Prefix (CP)** is added to each OFDM symbol. The CP is essentially a copy of the end of the symbol pasted at the beginning, creating a guard interval.

#### Uplink vs. Downlink Waveforms

<img width="1461" height="970" alt="image" src="https://github.com/user-attachments/assets/300ee545-ac85-4565-8e98-b3f0d3efba76" />

While the downlink uses standard OFDM, the uplink has two options:
* **CP-OFDM**: Identical to the downlink waveform.
* **DFT-Precoded OFDM (also known as SC-FDMA)**: This is a variation where the data undergoes a DFT (Discrete Fourier Transform) precoding step before the standard OFDM modulation. The key benefit of this is a **lower Peak-to-Average Power Ratio (PAPR)**. A high PAPR requires more expensive and less power-efficient amplifiers, which is a major constraint for battery-powered devices. Using DFT-precoded OFDM in the uplink helps to conserve the device's battery life.

---

### Multiple Access Scheme

A multiple access scheme is the technique that allows multiple mobile users to share the available radio spectrum efficiently.

<img width="1558" height="817" alt="image" src="https://github.com/user-attachments/assets/6b4b909e-bbf3-449d-8567-d4f802e267aa" />

* **OFDMA (Orthogonal Frequency-Division Multiple Access)**: This is the primary multiple access scheme in 5G NR. It's a multi-user version of OFDM where different users are allocated different subsets of the available subcarriers. This allows for very flexible and granular resource allocation in both the time and frequency domains.
* **DFT-Precoded OFDMA**: This is the multi-user version of the DFT-precoded OFDM waveform used in the uplink. It shares the same principle of allocating resources but ensures a lower PAPR for the transmitting devices.

---

### Flexible Numerology

A defining feature of 5G NR is its **flexible numerology**. This means that the subcarrier spacing (SCS) is not fixed but can be scaled to suit different deployment scenarios and frequency bands.

<img width="1432" height="822" alt="image" src="https://github.com/user-attachments/assets/1e705252-8a45-4793-b224-eb339fc0c44b" />

The key trade-offs are:
* **Large Subcarrier Spacing** (e.g., 120 kHz, 240 kHz):
    * **Pros**: Less sensitive to frequency errors (phase noise). Shorter symbol duration, which is better for low-latency applications.
    * **Cons**: The cyclic prefix becomes a larger portion of the symbol, making it less efficient.
* **Small Subcarrier Spacing** (e.g., 15 kHz, 30 kHz):
    * **Pros**: More efficient use of the cyclic prefix.
    * **Cons**: More sensitive to frequency errors.

This flexibility allows NR to operate efficiently across a vast range of frequencies (from sub-1 GHz to millimeter wave) and for various cell sizes and service types.

---

### Time-Domain Structure

<img width="1651" height="949" alt="image" src="https://github.com/user-attachments/assets/fd177e5d-1947-49b7-9eb8-48320658df9f" />

The 5G NR time domain is structured hierarchically:
* **Frame**: A fixed duration of **10 ms**.
* **Subframe**: Each frame is divided into 10 subframes, each **1 ms** long.
* **Slot**: The number of slots per subframe depends on the numerology (subcarrier spacing). A slot always consists of **14 OFDM symbols**. As the subcarrier spacing increases, the symbol duration decreases, so more slots can fit into a 1 ms subframe. For example:
    * 15 kHz SCS: 1 slot per subframe
    * 30 kHz SCS: 2 slots per subframe
    * 60 kHz SCS: 4 slots per subframe
    * 120 kHz SCS: 8 slots per subframe

#### Mini-Slots

<img width="1572" height="925" alt="image" src="https://github.com/user-attachments/assets/b20f4ac1-6df7-448a-9b39-cf1b4ed18ae8" />

For applications requiring extremely low latency, waiting for a full slot boundary to start a transmission can be too slow. To address this, NR introduces the concept of **mini-slots**. A mini-slot can be shorter than a full slot (2, 4, or 7 symbols long) and can start at any symbol boundary, allowing for much faster and more agile scheduling.

---

### Resource Grid

<img width="1343" height="941" alt="image" src="https://github.com/user-attachments/assets/30be103a-d8ea-409c-879b-d3f077a32efa" />

The fundamental unit of the 5G resource grid is the **Resource Element (RE)**, which represents one subcarrier in the frequency domain for the duration of one OFDM symbol in the time domain.

For scheduling purposes, Resource Elements are grouped into **Resource Blocks (RBs)**. One Resource Block consists of **12 consecutive subcarriers** in the frequency domain.

# 2.8 RRC and NAS

<img width="1484" height="883" alt="image" src="https://github.com/user-attachments/assets/0366a41b-1c61-45e0-a308-24bcd2507eaf" />

In the 5G architecture, the control plane is managed by two key protocols that operate at different levels of the network stack:

* **Non-Access Stratum (NAS)**: This protocol handles the communication between the User Equipment (UE) and the core network's Access and Mobility Management Function (AMF). It is responsible for functions that are independent of the radio access technology, such as:
    * Authentication and security procedures.
    * Managing idle-mode behavior, like paging.
    * Assigning IP addresses to devices.

* **Radio Resource Control (RRC)**: This protocol governs the communication between the UE and the gNodeB (the 5G base station). It manages all aspects of the radio connection, including:
    * Broadcasting essential system information.
    * Establishing, maintaining, and tearing down the radio connection.
    * Controlling device mobility within the radio network.
    * Configuring and receiving measurement reports from the device.
    * Managing the device's radio capabilities.

---

### RRC States

<img width="1620" height="980" alt="image" src="https://github.com/user-attachments/assets/7090ff13-1f52-497b-ace5-bd7344a817a0" />

To efficiently manage device resources and power consumption, a UE in the 5G network can be in one of three RRC states:

#### 1. RRC IDLE

This is the initial state of the device after it is powered on.

* **Characteristics**:
    * The device is not registered with the network.
    * There is no active RRC connection (no RRC context).
* **Behavior**: In this state, the UE is mostly "sleeping" to conserve battery. It periodically wakes up to monitor for paging messages from the network, which would alert it to an incoming call or data.

#### 2. RRC CONNECTED

When the device needs to actively send or receive data, it moves from IDLE to the CONNECTED state.

* **Characteristics**:
    * An RRC connection is established between the UE and the gNodeB.
    * The device is registered with the network and has a known location at the cell level.
* **Behavior**: In this state, the UE is actively communicating with the network, and seamless handovers between cells are managed by the network to ensure uninterrupted service.

#### 3. RRC INACTIVE

The INACTIVE state is a new addition in 5G, designed to offer a middle ground that combines the power efficiency of the IDLE state with the quick connection resumption of the CONNECTED state.

* **Characteristics**:
    * The RRC context (the device's radio configuration and security information) is stored in both the UE and the last serving gNodeB.
    * The connection to the core network is maintained.
* **Behavior**: This state allows the UE to transition back to the CONNECTED state very quickly (**RRC Resume**) without the need for the full connection setup procedure from IDLE. This is highly beneficial for applications that have sporadic data transfers, as it significantly reduces latency and signaling overhead. While in this state, the device can move around a predefined set of cells (a RAN Notification Area) without needing to update the network of its location.

---

### Mobility Management

<img width="1618" height="917" alt="image" src="https://github.com/user-attachments/assets/c04687ae-3f33-4b64-b81d-62c68d47d7bb" />

Mobility management ensures that a device stays connected as it moves through the network. The strategy for managing this depends on the RRC state of the device.

#### Idle and Inactive Mode Mobility

In both the IDLE and INACTIVE states, mobility is **UE-controlled**.

* **Tracking Areas (TA)**: The core network groups cells into larger **Tracking Areas**. When a device in IDLE mode moves into a new TA, it must perform a **NAS Registration Update** to inform the core network of its new location.
* **RAN Notification Areas (RNA)**: The radio access network (RAN) groups cells into **RAN Notification Areas**. A device in the INACTIVE state can move freely between cells within its assigned RNA without needing to contact the network. Only when it moves to a cell outside of its current RNA does it need to perform an **RRC RAN Notification Area Update**.

This hierarchical approach reduces the amount of signaling required, as the device only needs to update the network when it crosses the boundary of a larger geographical area.

#### Connected Mode Mobility

<img width="1185" height="898" alt="image" src="https://github.com/user-attachments/assets/e1b63b64-fe9f-4215-b31a-7f025c98311b" />

In the RRC CONNECTED state, mobility is entirely **network-controlled**.

* The UE continuously measures the signal strength of its current (serving) cell and neighboring cells using reference signals (SSB).
* It reports these measurements back to the gNodeB.
* Based on these reports, the network makes the decision about when and where to perform a **handover**, seamlessly transferring the device's connection from one cell to another to maintain the best possible link quality.

# 3.  Key RAN Procedures

# 3.1 Initial Access

When a 5G device is powered on, the very first thing it needs to do is find and synchronize with a nearby 5G cell. This entire process is known as **Initial Access**.

---

### Cell Search

<img width="1085" height="829" alt="image" src="https://github.com/user-attachments/assets/21c16865-922e-4b6e-b23e-00450bf06850" />

The primary goal of the cell search procedure is for the User Equipment (UE) to achieve time and frequency synchronization with a cell and to identify that cell's unique **Physical Cell ID (PCI)**.

To facilitate this, each 5G cell broadcasts a **Synchronization Signal Block (SSB)**. The SSB is a special block of signals that contains three key components:
* **Primary Synchronization Signal (PSS)**
* **Secondary Synchronization Signal (SSS)**
* **Physical Broadcast Channel (PBCH)**

The PSS and SSS are used together to determine the cell's PCI, while the PBCH carries the most essential system information that the device needs to connect to the network.

<img width="1409" height="854" alt="image" src="https://github.com/user-attachments/assets/7a9ff564-758f-4e29-8597-a6f7b6c7e2f7" />

#### SSB Transmission

In 5G, the SSB is not always transmitted from the center of the cell's bandwidth. To cover a wide area, especially at higher frequencies, SSBs can be transmitted in different directions using a technique called **beamforming**. A set of these directionally transmitted SSBs is called an **SSB Burst Set**.

---

### The Cell Search Process in Detail

The cell search is a multi-step process:

#### 1. Scan for the Primary Synchronization Signal (PSS)

When a device is first turned on, it doesn't know where the 5G carrier frequencies are. It begins by scanning a range of possible frequencies, looking for the PSS.

<img width="1516" height="901" alt="image" src="https://github.com/user-attachments/assets/95e2c6b8-f6e6-41b8-b5bc-d207230db92b" />

To make this scanning process faster and more efficient, 5G introduced a concept called the **Synchronization Raster**. This is a sparse grid of frequencies where the SSB is guaranteed to be found. Instead of scanning the entire dense **Carrier Raster** (which has a 100 kHz spacing), the UE only needs to check the points on the much wider Synchronization Raster (1.2 or 1.4 MHz spacing). This significantly speeds up the initial search.

Once the PSS is found, the device achieves initial time and frequency synchronization and also learns a part of the Physical Cell ID, specifically a value between {0, 1, 2}.

#### 2. Scan for the Secondary Synchronization Signal (SSS)

After detecting the PSS, the UE knows the exact location of the SSS within the same SSB. It then decodes the SSS to obtain the second part of the Physical Cell ID, which is a value between 0 and 335.

<img width="1028" height="947" alt="image" src="https://github.com/user-attachments/assets/c3dfaa3e-3b4b-4fc7-bd60-562a293d2d09" />

By combining the information from both the PSS and SSS, the UE can calculate the complete **Physical Cell ID (PCI)** for the cell. There are a total of 1008 unique PCIs available in 5G NR.

#### 3. Decode the Physical Broadcast Channel (PBCH) for the MIB

<img width="1364" height="880" alt="image" src="https://github.com/user-attachments/assets/a3a18b54-f264-42d1-892a-23be925e1b7d" />

Now that the UE is synchronized and knows the cell's ID, it can decode the Physical Broadcast Channel (PBCH), which is also located within the SSB. The PBCH carries the **Master Information Block (MIB)**.

The MIB contains the most critical system information, including:
* The system's bandwidth.
* The System Frame Number (SFN), which helps with timing.
* Information on whether the cell is barred (not allowing connections).
* Parameters needed to find and decode the next piece of crucial information: **System Information Block 1 (SIB1)**.

#### 4. Decode System Information Block 1 (SIB1)

<img width="1311" height="862" alt="image" src="https://github.com/user-attachments/assets/0fadf0ae-c346-430c-a094-961367e58b95" />

Using the information from the MIB, the UE can find and decode SIB1. SIB1 is also considered part of the **Remaining Minimum System Information (RMSI)** and contains essential information for the UE to access the cell, such as:
* Cell selection information.
* Cell access-related information.
* Information about where to find other, less critical SIBs.

At this point, the UE has enough information to decide whether it wants to "camp" on this cell and attempt to connect.

#### 5. Acquiring Other SIBs

<img width="1557" height="917" alt="image" src="https://github.com/user-attachments/assets/55e0016d-10d4-4abb-8e4a-6401c238a80a" />

Other System Information Blocks (SIBs) contain less essential information that is not immediately needed for initial access, such as details for cell re-selection to other frequencies or other radio technologies (like LTE). These can be broadcast periodically by the network or provided to the device on-demand when requested.

<img width="819" height="875" alt="image" src="https://github.com/user-attachments/assets/efbdc0e3-436b-471f-af26-2a269ac56999" />

# 3.2 Random Access
## 5G NR: Random Access Procedure

After a device has successfully synchronized with a cell and read the initial system information, it needs to perform a **Random Access (RA)** procedure to establish a connection with the network.

---

### When is Random Access Triggered?

A device will initiate the Random Access procedure in several situations:
* When it needs to transition from an idle state to a connected state to send or receive data.
* When it is already connected but has lost its uplink synchronization.
* During a handover to a new cell.

---

### The 4-Step Random Access Procedure

The most common type of random access is the **4-step Contention-Based Random Access (CBRA)**. It's called "contention-based" because multiple devices might try to access the network at the same time, leading to potential collisions.

<img width="1200" height="754" alt="image" src="https://github.com/user-attachments/assets/f562ef09-bc74-43db-965a-bda50f5688f3" />

The procedure involves four key messages exchanged between the User Equipment (UE) and the gNodeB:

#### Step 1: Message 1 - Random Access Preamble

<img width="1565" height="950" alt="image" src="https://github.com/user-attachments/assets/e2bb47d9-40ac-4b00-97c8-85998e8b524c" />

* **What it is**: The UE sends a randomly selected **preamble** sequence to the gNodeB. This preamble is like a "hello" message, signaling the network that the device wants to connect.
* **Key Information**:
    * The UE uses a specific physical channel called the **Physical Random Access Channel (PRACH)** for this transmission.
    * It also performs initial **timing adjustments** based on its measurements of the cell's synchronization signals (SSB) to ensure the preamble arrives at the gNodeB at the correct time.

#### Step 2: Message 2 - Random Access Response (RAR)

<img width="1638" height="866" alt="image" src="https://github.com/user-attachments/assets/0a947926-6f10-42cb-b116-358f7e96c26b" />

* **What it is**: The gNodeB, upon detecting the preamble, sends back a **Random Access Response (RAR)**.
* **Key Information**:
    * **Preamble Identifier**: The RAR indicates which preamble it is responding to.
    * **Timing Correction**: It provides a precise timing advance command to correct any remaining synchronization errors.
    * **Temporary ID (TC-RNTI)**: A temporary identifier is assigned to the UE for the duration of the random access procedure.
    * **Uplink Grant**: It gives the UE an initial grant of uplink resources (time and frequency blocks) to use for the next step.

#### Step 3: Message 3 - RRC Connection Request

<img width="1664" height="772" alt="image" src="https://github.com/user-attachments/assets/3b490898-ef8e-4535-a150-702c1553abc2" />

* **What it is**: Using the uplink resources granted in the RAR, the UE sends its first scheduled message to the gNodeB. This is an **RRC Connection Setup Request**.
* **Key Information**: This message includes a unique identifier for the UE. This is crucial for the next step, **contention resolution**. If two devices happened to choose the same preamble in Step 1, they would both receive the same RAR. By sending their unique IDs in this step, the network can tell them apart.

#### Step 4: Message 4 - Contention Resolution

<img width="1544" height="769" alt="image" src="https://github.com/user-attachments/assets/dd3515c2-83af-46c0-9305-7f3fc7e922c8" />

* **What it is**: The gNodeB sends a final message to resolve any potential contention and confirm the connection.
* **Key Information**:
    * This message is addressed to the UE using its temporary ID (TC-RNTI).
    * Crucially, the message contains the **unique UE ID** that was sent in Step 3.
    * When the UE receives this message and sees its own unique ID, it knows that it has successfully won the contention and the random access procedure is complete. It is now in an **RRC Connected** state.
    * If another device was contending for the same resource, it will not see its ID in this message and will know that its access attempt has failed, prompting it to go back to Step 1 and try again.

---

### Contention-Free Random Access (CFRA)

<img width="517" height="792" alt="image" src="https://github.com/user-attachments/assets/23127a79-542c-42d7-a4eb-142156e2f5bf" />

There is also a **Contention-Free Random Access (CFRA)** procedure. This is used in specific scenarios where the network wants to initiate contact with a device without the risk of collision, such as:
* During a handover procedure.
* When there is downlink data waiting for a specific UE.

In this case, the gNodeB pre-assigns a dedicated, unique preamble to the UE. Since no other device will use this preamble, there is no possibility of contention, making the process faster and more reliable.

<img width="1155" height="721" alt="image" src="https://github.com/user-attachments/assets/8a87ceab-a911-498b-b2fc-71c15ca83bba" />

# 4. 5G Core Networks

# 4.1 5G Core Network: Identifiers

In the 5G ecosystem, a variety of identifiers are used to distinguish between devices and individual subscriptions, ensuring that data is routed correctly and securely.

<img width="783" height="876" alt="image" src="https://github.com/user-attachments/assets/8af9d9c1-c7aa-4e5f-9a8f-92f0243f24f9" />

---

### Device vs. Subscription Identity

It's important to differentiate between two main types of identifiers:

* **Device Identity**: This is tied to the physical piece of hardware, the User Equipment (UE). The primary identifier for this is the **PEI**.
* **Subscription Identity**: This is linked to the user's subscription with the mobile network operator. The core identifiers here are the **SUPI** and **SUCI**, with the **GUTI** used for temporary tracking.

---

### Device Identifier

#### PEI (Permanent Equipment Identifier)

<img width="1536" height="964" alt="image" src="https://github.com/user-attachments/assets/66018f2b-9708-472a-85a4-72658af86b2c" />

* **What it is**: The PEI is the unique serial number that identifies a physical mobile device. In most mobile devices, this is the **IMEI** (International Mobile Station Equipment Identity) or **IMEISV** (which also includes the software version).
* **Key Characteristics**:
    * It is permanently stored in the device.
    * It is transmitted over the network only in specific situations, such as for emergency calls, to maintain security.

---

### Subscription Identifiers

<img width="1577" height="897" alt="image" src="https://github.com/user-attachments/assets/ae27bc10-292e-4649-a876-03738d95e194" />

#### SUPI (Subscription Permanent Identifier)

* **What it is**: The SUPI is the globally unique and permanent identifier for a user's subscription. In the context of traditional mobile networks, the SUPI is the **IMSI** (International Mobile Subscriber Identity).
* **IMSI Structure**:
    * **MCC (Mobile Country Code)**: A 3-digit code that identifies the country.
    * **MNC (Mobile Network Code)**: A 2 or 3-digit code for the specific network operator within that country.
    * **MSIN (Mobile Subscriber Identification Number)**: The remaining digits uniquely identify the subscriber on that network.

#### SUCI (Subscription Concealed Identifier)

<img width="1370" height="926" alt="image" src="https://github.com/user-attachments/assets/12ca2236-efe2-4e7a-9d22-62883b75a2b7" />

* **Why it's needed**: To enhance privacy and prevent tracking, the permanent SUPI (IMSI) is rarely sent over the radio network in an unencrypted format. Sending it openly would make users vulnerable to "IMSI Catchers," which are devices that can intercept this identifier to track a user's location and activity.
* **What it is**: Before being sent over the air, the SUPI is encrypted using a "protection scheme." The resulting encrypted value is the **SUCI**. This ensures that even if the identifier is intercepted, it cannot be used to identify the subscriber.

#### GUTI (Globally Unique Temporary Identifier)

<img width="1395" height="834" alt="image" src="https://github.com/user-attachments/assets/b489b0f8-39dd-4125-903e-9c15e0209cd4" />

* **What it is**: To avoid sending the SUPI/SUCI frequently, the network assigns a temporary identifier to the device called the **GUTI**. This is a temporary ID that can be changed by the network at any time for security.
* **Structure**: The GUTI is composed of two main parts:
    * **GUAMI (Globally Unique AMF Identifier)**: This identifies the specific Access and Mobility Management Function (AMF) in the core network that is currently serving the device. The GUAMI itself is made up of the MCC, MNC, and an AMF Identifier.
    * **5G-TMSI (5G Temporary Mobile Subscriber Identity)**: This is the temporary identifier for the device within that specific AMF.




# **SUMMARY** 5G core networks file no. 4

## 5G Core Network: An Overview

The 5G Core Network introduces a **Service-Based Architecture (SBA)**, which is a major shift from the architecture of previous mobile generations. Instead of monolithic network elements with fixed interfaces, the 5G core is built on the principles of **microservices**, where each **Network Function (NF)** is a modular, independent component that offers its services to other NFs through well-defined, web-based APIs.

This cloud-native approach makes the network highly flexible, scalable, and easier to upgrade and maintain.

---

### Key Network Functions (NFs) in the 5G Core

Here are the roles of the main Network Functions in the 5G Core:

#### AMF (Access and Mobility Management Function)

The AMF is the primary control point for managing the device's connection to the network. Its main responsibilities are:

* **Registration Management**: Handles the process of a device registering and de-registering with the network, which includes authenticating the user.
* **Connection Management**: Establishes, maintains, and releases the control plane connections between the device and the core network.
* **Mobility Management**: Tracks the device's location and manages handovers between base stations (gNodeBs) to ensure seamless connectivity as the user moves.



---

#### SMF (Session Management Function)

The SMF is responsible for all aspects related to the user's data sessions. A **PDU (Packet Data Unit) Session** is essentially the logical connection that provides the user with access to a data network, like the internet.

The SMF's key functions include:
* **PDU Session Management**: It handles the setup, modification, and release of PDU sessions.
* **IP Address Allocation**: It assigns an IP address (IPv4, IPv6, or both) to the device for its data session.
* **UPF Selection**: It selects the appropriate User Plane Function (UPF) to handle the user's data traffic.
* **Policy Enforcement**: It works with the PCF to enforce Quality of Service (QoS) and other policies for the data session.

---

#### UPF (User Plane Function)

The UPF is the workhorse of the user data plane. It is responsible for forwarding the actual user traffic between the radio access network (the gNodeB) and the external data network (e.g., the internet).

Its main functions are:
* **Packet Routing and Forwarding**: It routes and forwards user data packets.
* **Policy Enforcement**: It applies the rules and policies defined by the SMF and PCF, such as Quality of Service (QoS) marking.
* **Mobility Anchor**: It acts as the anchor point for the PDU session, ensuring that the user's IP address remains the same even when they move between different base stations.



---

#### UDM and UDR (Unified Data Management and Unified Data Repository)

These two functions work together to manage all the subscription data in the 5G network. This separation of the application logic from the data storage is a key principle of the service-based architecture.

* **UDR (Unified Data Repository)**: This is the centralized database that securely stores all the subscription data, policy data, and other network information.
* **UDM (Unified Data Management)**: This function acts as the front-end to the UDR. It provides the application logic for managing and accessing the subscription data, including functions for authentication and access authorization.

---

#### PCF (Policy Control Function)

The PCF is responsible for defining and managing the policies that govern the behavior of the network and the services provided to users. These policies can be applied at different levels, from all users on the network to a specific data flow for a single user.

The PCF manages two main types of policies:
* **Access and Mobility Policies**: These include rules for things like service area restrictions and which radio technologies a user is allowed to access.
* **Session Management Policies**: These are rules related to data sessions, such as:
    * **Gating Control**: Deciding whether to allow or block certain types of data traffic.
    * **QoS Control**: Defining the Quality of Service for different data flows, ensuring that high-priority traffic gets the necessary resources.

# **SUMMARY** 5G call flows file NO. 5

## 5G Core Network: Key Procedures

This document outlines some of the fundamental procedures that manage a device's lifecycle in a 5G network, from connecting to the network to disconnecting and establishing data sessions.

---

### Registration Procedure

The **Registration Procedure** is how a User Equipment (UE) gets authorized to use the 5G network. This procedure is always initiated by the UE and can be triggered for several reasons:

* **Initial Registration**: Occurs when a UE is powered on and needs to connect to the network for the first time.
* **Mobility Registration**: Triggered when a UE moves into a new Tracking Area (a group of cells) and needs to update the network with its new location.
* **Periodic Registration**: The UE periodically re-registers with the network to signal that it is still active.
* **Emergency Registration**: A special type of registration for accessing emergency services.

#### The Registration Process

1.  The UE sends a **Registration Request** to the Radio Access Network (RAN), which forwards it to the Access and Mobility Management Function (AMF).
2.  If the UE is moving from an area served by a different AMF, the new AMF will fetch the UE's context (its current state and security information) from the old AMF.
3.  The AMF then initiates **authentication and security** procedures to verify the identity of the user.
4.  The AMF updates the Unified Data Management (UDM) with the UE's registration status and subscribes to notifications for any changes in the subscription data.
5.  Policy control rules are created by the Policy Control Function (PCF).
6.  The AMF sends a **Registration Accept** message back to the UE, confirming that it is now successfully registered with the network. This message may also include a new temporary identifier (GUTI) for the UE.

---

### PDU Session Establishment

Once a UE is registered, it can request to establish a **Packet Data Unit (PDU) Session**. This is the logical connection that allows the UE to exchange data packets with an external Data Network (DN), like the internet.

This procedure can be initiated by the UE or, in some cases, triggered by the network.

#### The PDU Session Establishment Process

1.  The UE sends a **PDU Session Establishment Request** to the AMF.
2.  The AMF selects a Session Management Function (SMF) to handle the data session and forwards the request.
3.  The SMF interacts with the UDM to retrieve the user's subscription data related to data sessions.
4.  The SMF communicates with the PCF to get the relevant policy and Quality of Service (QoS) rules for this session. It also selects a User Plane Function (UPF) that will handle the user's data traffic.
5.  The SMF sends a message to the AMF to establish the user plane resources between the RAN and the selected UPF.
6.  The RAN configures the radio resources for the UE, establishing the data path.
7.  The SMF confirms the establishment of the session with the UPF.
8.  The UE is now able to send and receive data.

---

### Deregistration Procedure

Deregistration is the process of disconnecting a UE from the network services. This can be initiated either by the UE (e.g., when the device is powered off) or by the network (e.g., due to subscription changes).

#### The Deregistration Process

1.  A **Deregistration Request** is sent to the AMF.
2.  The AMF initiates the release of any active PDU Sessions by communicating with the corresponding SMF.
3.  The SMF releases the session with the PCF and the UPF.
4.  The AMF informs the UDM that the UE is now deregistered.
5.  A **Deregistration Accept** message is sent back to the UE.
6.  The signaling connection between the UE and the AMF is released, and the device transitions to a deregistered state.
