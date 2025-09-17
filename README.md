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

#### **Target Audience**
* Telecom Professionals who want to learn about the 5G RAN.
* Students who are interested in joining the telecommunications industry.

#### **Prerequisites**
* A basic understanding of the principles of networks.
* A basic understanding of wireless communications.

#### **Learning Outcomes & Course Structure**
* At the end of the course, you will be able to work with advanced concepts that are part of the 5G RAN.
* The course is structured to make complex ideas simple to understand, using visual illustrations where necessary.

# 2. The 5G standardization

***

## 1. Introduction: The Need for Standardization

The development of a global technology like 5G raises two fundamental questions:
1.  **Who defines what 5G is?**
2.  **Who actually designs the technology for 5G?**

The process that answers these questions is **standardization**.

### The Power Outlet Analogy 🔌

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

# 3. The 5G use cases

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


# 4. Overview of the 5G System Architecture

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






