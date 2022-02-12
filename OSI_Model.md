# OSI Model

### **ABSTRACTION**

The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software. In the OSI reference model, the communications between a computing system are split into seven different abstraction layers.

Created at a time when network computing was in its infancy, the OSI was published in 1984 by the International Organization for Standardization (ISO). Though it does not always map directly to specific systems, the OSI Model is still used today as a means to describe Network Architecture.

<br>

### **1. INTRODUCTION**
The International Standard Organization (ISO) is a multinational body dedicated to a worldwide agreement on international standards which was established in 1947. The ISO proposed a model named OSI (Open System Interconnection) in 1983, which covers all aspects of network communication.

<br>

 The purpose of the OSI model is for open communication between different systems without requiring changes to the logic of the underlying hardware and software. The OSI model is not a protocol, it is a model for understanding and designing a network architecture that is flexible, robust, and interoperable. 

 <br>
 
### **2. DEFINITION**
The open systems interconnection (OSI) model is a conceptual model created by the International Organization for Standardization which enables diverse communication systems to communicate using standard protocols. In plain English, the OSI provides a standard for different computer systems to be able to communicate with each other.
<br>
<br>

### **3. CHARACTERISTICS OF OSI MODEL**
The OSI model is divided into two layers: Upper layers and Lower layers.
* **Upper Layer:**
The upper layer of the OSI model mainly deals with application-related issues, and they are implemented only in the software. The application layer is closest to the end-user. Both the end-user and the application layer interact with the software applications.

* **Lower Layer:** 
The lower layer of the OSI model deals with data transport issues. The data link layer and the physical layer are implemented in hardware and software. The physical layer is the lowest layer of the OSI model and is closest to the physical medium.

<br>

### **4. ARCHITECTURE OF OSI MODEL**
There are seven OSI layers. Each layer has different functions. A list of seven layers is given below.


![OSI Modal Architecture](https://insights.profitap.com/hs-fs/hubfs/The%207%20Layers%20of%20OSI.png?width=560&name=The%207%20Layers%20of%20OSI.png "OSI Modal Architecture") 


### **4.1. Physical Layer**
The lowest layer of the OSI reference model is the physical layer. It is responsible for the actual physical connection between the devices. The physical layer contains information in the form of bits. It is responsible for transmitting individual bits from one node to the next. 

Hub, Repeater, Modem, Cables are some examples of physical layer devices. 

The functions of the physical layer are :
* **Bit synchronization:** The physical layer provides the synchronization of the bits by providing a clock. This clock controls both sender and receiver thus providing synchronization at bit level.

* **Bit rate control:** The Physical layer also defines the transmission rate i.e. the number of bits sent per second.

* **Physical topologies:** Physical layer specifies the way in which the different, devices/nodes are arranged in a network i.e. bus, star, or mesh topology.

* **Transmission mode:** Physical layer also defines the way in which the data flows between the two connected devices. The various transmission modes possible are Simplex, half-duplex and full-duplex.



### **4.2. Data Link Layer (DLL)**
The data link layer is responsible for the node-to-node delivery of the message. The main function of this layer is to make sure data transfer is error-free from one node to another, over the physical layer. 


Data Link Layer is divided into two sublayers:

* Logical Link Control (LLC)

* Media Access Control (MAC)

The functions of the Data Link layer are :

* **Framing:** It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.

* **Physical addressing:** After creating frames, the Data link layer adds physical addresses (MAC address) of the sender and/or receiver in the header of each frame.

* **Error control:** Data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.

* **Flow Control:** The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates the amount of data that can be sent before receiving an acknowledgment.

* **Access control:** When a single communication channel is shared by multiple devices, the MAC sub-layer of the data link layer helps to determine which device has control over the channel at a given time.

### **4.3. Network Layer**
The network layer works for the transmission of data from one host to the other located in different networks. It also takes care of packet routing i.e. selection of the shortest path to transmit the packet, from the number of routes available. 

The functions of the Network layer are :
* **Routing:** The network layer protocols determine which route is suitable from source to destination. This function of the network layer is known as routing.

* **Logical Addressing:** In order to identify each device on internetwork uniquely, the network layer defines an addressing scheme. The sender & receiver's IP addresses are placed in the header by the network layer. Such an address distinguishes each device uniquely and universally.

### 4.4. **Transport Layer**
The transport layer provides services to the application layer and takes services from the network layer. The data in the transport layer is referred to as Segments. It is responsible for the End to End Delivery of the complete message. 

* **A sender's side:**
The transport layer receives the formatted data from the upper layers, performs segmentation, and also implements flow and error-free control to ensure proper data transmission. It also adds Source and Destination port numbers in its header and forwards the segmented data to the Network Layer. 

* **At receiver's side:** 
Transport Layer reads the port number from its header and forwards the Data that it has received to the respective application. It also performs sequencing and reassembling of the segmented data.

The functions of the transport layer are :
* **Segmentation and Reassembly:** This layer accepts the message from the (session) layer, breaks the message into smaller units. Each of the segments produced has a header associated with it. The transport layer at the destination station reassembles the message.

* **Service Point Addressing:** In order to deliver the message to the correct process, the transport layer header includes a type of address called service point address or port address. Thus by specifying this address, the transport layer makes sure that the message is delivered to the correct process.

### **4.5. Session Layer**
This layer is responsible for the establishment of connection, maintenance of sessions, authentication, and also ensures security.
 

The functions of the session layer are :
* **Session establishment, maintenance, and termination:** The layer allows the two processes to establish, use and terminate a connection.

* **Synchronization:** This layer allows a process to add checkpoints which are considered synchronization points into the data. These synchronization points help to identify the error so that the data is re-synchronized properly, ends of the messages are not cut prematurely and data loss is avoided.

* **Dialog Controller:** The session layer allows two systems to start communication with each other in half-duplex or full-duplex.

### **4.6. Presentation Layer**
The presentation layer is also called the Translation layer. The data from the application layer is extracted here and manipulated as per the required format to transmit over the network. 

The functions of the presentation layer are :
* **Translation:** For example, ASCII to EBCDIC.

* **Encryption/ Decryption:** Data encryption translates the data into another form or code. The encrypted data is known as the ciphertext and the decrypted data is known as plain text. 

* **Compression:** Reduces the number of bits that need to be transmitted on the network.

### **4.7. Application Layer**
At the very top of the OSI Reference Model stack of layers, we find the Application layer which is implemented by the network applications. 

These applications produce the data, which has to be transferred over the network. This layer also serves as a window for the application services to access the network and for displaying the received information to the user. 

Ex: Application - Browsers, Skype Messenger, etc. 

The functions of the Application layer are :

* Network Virtual Terminal
* FTAM-File transfer access and management
* Mail Services
* Directory Services

<br>

### **5. CONCLUSION**
The International Standard Organization created a model called the open system interconnection, which allows the diverse systems to communicate. The seven-layer OSI model provides guidelines for the development of universally compatible networking protocols.

<br>

### **6. REFERENCE**
* https://www.youtube.com/watch?v=vv4y_uOneC0
* https://en.wikipedia.org/wiki/OSI_model
* https://www.javatpoint.com/osi-model
* https://insights.profitap.com/hs-fs/hubfs/The%207%20Layers%20of%20OSI.png


