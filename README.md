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
<img width="1651" height="871" alt="image" src="https://github.com/user-attachments/assets/e91affd2-3e00-4d28-a55b-6917e1a703e3" />

* **Option 4 (NE-DC)**: This is the reverse of Option 3. It uses the **5G Core**, with the **gNodeB as the master node** for control signaling and the **eNodeB as a secondary data booster**. This becomes relevant when 5G coverage is mature and becomes the primary network.

  <img width="1674" height="1001" alt="image" src="https://github.com/user-attachments/assets/2672432c-c56b-42ef-91d3-592f94e07eac" />

  <img width="1029" height="897" alt="image" src="https://github.com/user-attachments/assets/5fccc732-f5a3-4491-92d8-60519aea1f37" />


* **Option 5**: An upgraded 4G base station, called an **eLTE eNodeB**, connects directly to the **5G Core**.

  <img width="1272" height="922" alt="image" src="https://github.com/user-attachments/assets/e2dbdfc4-996f-4aea-832c-04964d929534" />

* **Option 7**: A variation where an eLTE eNodeB connects to the **5G Core** and acts as the master node, with a gNodeB serving as the secondary node.

  <img width="1201" height="982" alt="image" src="https://github.com/user-attachments/assets/12f3effa-ef92-4987-b64c-225547eb0695" />

* **Option 6**: A configuration where a 5G gNodeB would connect to a 4G Core. This option is **not supported** by the standards.

  ![Uploading image.png…]()


# 2. 5G RAN Protocol Stack

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








