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
