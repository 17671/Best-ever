# Module: Hardware, Networks and Behaviorist AI

## Chapter 1: Hardware

### Chapter Overview

This chapter introduces what a computer is and how it works, from the basic workflow of input, processing, storage, and output down to the binary data it uses. You'll study number systems, data storage, and the Von Neumann model, then the physical components that make up a computer. The chapter ends with how a program runs and a simple computer (MARIE), and looks ahead to emerging trends in hardware.

### Learning Outcomes

By the end of this chapter, you will be able to:

1. Define a computer, describe its basic workflow, and distinguish between types of computers.
2. Convert between binary, decimal, octal, and hexadecimal number systems.
3. Explain how numbers, text, images, audio, and video are stored as binary data.
4. Describe the Von Neumann model and its main components.
5. Identify input, output, and internal hardware components, and explain the difference between internal and external hardware.
6. Apply hardware knowledge to a realistic case study.
7. Explain how hardware components work together to execute a program.
8. Describe the structure and operation of a simple computer (MARIE).
9. Recognize emerging trends in computer hardware.

---

## Contents

| Stage | Topic |
| --- | --- |
| [1](#stage-1-computers-and-data) | Computers and Data |
| [2](#stage-2-number-systems) | Number Systems |
| [3](#stage-3-data-storage) | Data Storage |
| [4](#stage-4-von-neumann-model) | Von Neumann Model |
| [5](#stage-5-computer-hardware) | Computer Hardware |
| [6](#stage-6-program-execution) | Program Execution |
| [7](#stage-7-a-simple-computer-marie) | A Simple Computer (MARIE) |
| [8](#stage-8-emerging-trends-in-hardware) | Emerging Trends in Hardware |

---

## Material

### Stage 1: Computers and Data

- Definition of a Computer
- The Basic Workflow of a Computer (input, processing, storage, output)
- Different Types of Computers (personal computers, servers, mobile devices, embedded systems, supercomputers)
- Chapter Exercise

### Stage 2: Number Systems

- Number System Overview
- Binary Number System
- Decimal to Binary and Binary to Decimal
- Octal to Binary and Binary to Octal
- Octal to Decimal and Decimal to Octal
- Hexadecimal to Binary and Binary to Hexadecimal
- Hexadecimal to Decimal and Decimal to Hexadecimal
- Chapter Exercise

### Stage 3: Data Storage

- Definition
- How Does Data Storage Work
- Representing Data in Binary (numbers, text, images, audio, video)
- Types of Data Storage (primary and secondary)
- Data Storage Devices (HDD, SSD, USB drives, optical discs)
- Cloud Storage Forms
- Chapter Exercise

### Stage 4: Von Neumann Model

- Definition
- Process (fetch-decode-execute)
- Components (1): CPU (control unit and ALU)
- Components (2): Memory, Input, and Output
- Advantages vs Disadvantages
- Chapter Exercise

### Stage 5: Computer Hardware

- Hardware Definition
- **Input Devices:** Mouse, Keyboard, Microphone, Camera, Touchpad
- **Output Devices:** Monitor, Printer, Speaker, Hearing Devices
- **Internal Hardware:** Motherboard, CPU, Hard Drive, Hard Drive Types, RAM, RAM vs ROM, Power Supply, Graphics Card, Graphics Card Components, Cooling System, Wi-Fi Card
- **Ports and External Storage:** USB, Memory Card
- Internal vs External Hardware
- Case Study: for example, choosing or diagnosing the components of a laptop or desktop for a given user need
- Chapter Exercise

### Stage 6: Program Execution

- Definition
- How Program Execution Works (from stored program to running task)
- Chapter Exercise

### Stage 7: A Simple Computer (MARIE)

- Definition: MARIE as a simple computer
- Process
- CPU (1): Structure
- CPU (2): Operation
- The Bus (1): Types of Bus (data, address, control)
- The Bus (2): How the Bus Transfers Data
- Memory
- Input and Output Devices
- Chapter Exercise

### Stage 8: Emerging Trends in Hardware

- Recent developments in processors and memory
- Trends in storage and connected devices
- How hardware trends affect networks (a bridge to the next chapter)

---



## Chapter 2: Networks

### Chapter Overview

A computer network connects two or more computers so they can share data and resources. This chapter covers the parts of a network, the types of network, how the internet works, the OSI model, network security, and emerging trends. Each stage breaks one topic into short steps.

| Term | Meaning |
| --- | --- |
| Network | Two or more connected devices that share data |
| Switch | Connects devices within one local network and forwards data to the right device |
| Router | Connects separate networks and chooses the path data takes |
| Packet | A small unit of data sent across a network |
| IP address | A numeric address that identifies a device on a network |
| Domain name | A readable name for a website, such as example.com |
| DNS | The system that converts domain names into IP addresses |
| URL | The full address of a web resource |
| Protocol | A set of rules for how devices communicate |
| Internet | The global network of connected networks |
| World Wide Web | The collection of pages and resources accessed over the internet |

### Learning Outcomes

By the end of this chapter, you will be able to:

1. Define a computer network and explain why computers are networked.
2. Identify the common parts of a network and describe what each does.
3. Distinguish PAN, LAN, MAN, and WAN, and describe the bus, star, ring, and mesh layouts.
4. Explain how the internet delivers data using TCP/IP, IP addresses, and domain names.
5. Read a URL and describe what happens between clicking a link and seeing the page.
6. Describe the seven layers of the OSI model and the job of each.
7. Explain privacy, authentication, integrity, and nonrepudiation, and match common protections to each.
8. Recognize emerging trends in networks and how they connect to AI.

---

## Contents

| Stage | Topic |
| --- | --- |
| [1](#stage-1-what-is-a-computer-network) | What Is a Computer Network? |
| [2](#stage-2-network-fundamentals) | Network Fundamentals |
| [3](#stage-3-internet-fundamentals) | Internet Fundamentals |
| [4](#stage-4-the-osi-model) | The OSI Model |
| [5](#stage-5-security-in-networks) | Security in Networks |
| [6](#stage-6-emerging-trends-in-networks) | Emerging Trends in Networks |

---

## Material

### Stage 1: What Is a Computer Network?

**Goal:** understand what a network is and why computers are connected.

1. **Network overview.** A network is two or more computers connected so they can exchange data.
2. **Why computers are networked.** To share data, to share resources such as a printer or storage, and to communicate.
3. **Check yourself.** Name two things you share over a network at home or school.

---

### Stage 2: Network Fundamentals

**Goal:** learn the parts, sizes, and layouts of networks.

1. **Devices.** Computers send and receive data. A server provides services to other computers. A switch connects devices within one local network. A router connects separate networks and chooses the path for data. A modem connects a network to the internet service provider. An access point provides wireless connections.
2. **Media.** Wired media carry data over cables. Wireless media carry data through radio signals.
3. **Network interface card.** The component that connects a device to a network.
4. **Types of network, by size.**
   - PAN (personal area network): devices around one person, such as a phone and earbuds.
   - LAN (local area network): one building or site, such as a home, school, or office.
   - MAN (metropolitan area network): a city or large campus.
   - WAN (wide area network): a large area such as a country or the world.
5. **Layouts (topologies).**
   - Bus: all devices share one main cable.
   - Star: each device connects to a central device.
   - Ring: each device connects to two neighbors in a loop.
   - Mesh: devices connect to many others, so there are several routes.
6. **Check yourself.** Draw a home network as a star and label the router.

---

### Stage 3: Internet Fundamentals

**Goal:** understand how data travels across the internet and how a web page reaches you.

1. **Internet vs the web.** The internet is the global network of connected networks. The World Wide Web is the collection of pages and resources accessed over it.
2. **TCP/IP.** TCP splits data into numbered packets, checks that all of them arrive, and puts them back in order. IP adds addresses to each packet and routes it.
3. **IP addresses.** Every connected device has a numeric address so data knows where to go.
4. **Domain names and DNS.** Domain names such as example.com are easier to remember than numbers. DNS converts a domain name into an IP address.
5. **URL, part 1: the parts.** A URL is the full address of a web resource. Example:

   ```text
   https://www.example.com/menu/pizza

   https            = protocol (the rules used to communicate)
   www.example.com  = domain name (which server)
   /menu/pizza      = path (which page on that server)
   ```

6. **URL, part 2: from click to page.**
   1. You click a link, which sends a request for a page.
   2. Your browser asks DNS for the server's IP address.
   3. Your request travels as packets to that address.
   4. The server sends the page back as packets.
   5. Your browser reassembles the packets and shows the page.
7. **Check yourself.** Explain the difference between a domain name and an IP address in one sentence.

---

### Stage 4: The OSI Model

**Goal:** learn the seven layers that organize network communication.

1. **What a layered model is.** Instead of one large job, network communication is split into seven smaller jobs. Each layer works with the layer above it and the layer below it.
2. **The seven layers, from top to bottom.**

   | Layer | Job | Examples |
   | --- | --- | --- |
   | 7. Application | Gives programs access to network services | Web browsing (HTTP), email |
   | 6. Presentation | Formats, compresses, and encrypts data | Encryption, character encoding, image formats |
   | 5. Session | Starts, maintains, and ends conversations between devices | Keeping a login session open |
   | 4. Transport | Splits data into segments and checks delivery | TCP, UDP |
   | 3. Network | Addresses data and routes it between networks | IP, routers |
   | 2. Data link | Delivers data between devices on the same link | Ethernet, Wi-Fi, switches |
   | 1. Physical | Sends raw bits as electrical, light, or radio signals | Cables, radio signals |

3. **How data moves.** On the sending device, data moves down the layers and each layer adds its own header information. On the receiving device, data moves up the layers and each layer removes its header.
4. **OSI vs TCP/IP.** OSI is a seven-layer reference model used for teaching and troubleshooting. TCP/IP is the shorter model the internet uses in practice, with fewer layers.
5. **Check yourself.** Which layer handles addressing, and which layer sends the raw signals?

---

### Stage 5: Security in Networks

**Goal:** learn the four security goals and common ways to protect a network.

1. **Why it matters.** Data crossing a network can be read, faked, or changed by others.
2. **Privacy (confidentiality).** Keeping data from people who are not allowed to read it. Encryption is the main protection.
3. **Authentication.** Proving who a user or device is, using passwords, codes, or other proofs.
4. **Integrity.** Making sure data has not been changed. Checksums and hashes compare data before and after it travels.
5. **Nonrepudiation.** Preventing someone from denying an action they took. Digital signatures and logs provide evidence.
6. **Common protections.** A firewall filters network traffic by rules. Encryption makes data unreadable without the key.
7. **Check yourself.** Match privacy, authentication, integrity, and nonrepudiation to one protection each.

---

### Stage 6: Emerging Trends in Networks

**Goal:** recognize where networks are heading and how that links to AI.

1. **Wireless and mobile.** Newer wireless and mobile networks offer higher speeds and support more connected devices.
2. **Cloud, Internet of Things, and edge.** Cloud computing provides remote servers over the internet. The Internet of Things connects everyday objects to networks. Edge computing processes data close to where it is produced.
3. **The bridge to Behaviorist AI.** More connected devices produce more data, which AI systems can learn from. The next chapter covers Behaviorist AI.

---

## Chapter 3: Behaviorist AI

### Chapter Overview

This chapter explains how an AI system can learn behavior from experience. You'll start with what Behaviorist AI is and the basics of reinforcement learning (RL). You'll then study Markov Decision Processes (MDPs) and the algorithms built on them. The chapter ends with how these methods are used in robotics and games, real-world applications, and the challenges and limitations of the approach.

### Learning Outcomes

By the end of this chapter, you will be able to:

1. Define Behaviorist AI and describe its basic process with an example.
2. Explain reinforcement learning in terms of agent, environment, actions, and rewards, and distinguish model-based from model-free learning.
3. Describe the parts of an MDP (states, actions, rewards, probabilities, policy, value function) and state the Bellman equation.
4. Explain dynamic programming, value iteration, and policy iteration.
5. Describe and compare the main RL algorithms (Q-learning, Deep Q-Network, SARSA, policy gradient, actor-critic) and on-policy versus off-policy learning.
6. Describe how RL is used in robotics and games.
7. Give examples of real-world applications of Behaviorist AI.
8. Identify the main challenges and limitations of Behaviorist AI.

---

## Contents

| Stage | Topic |
| --- | --- |
| [1](#stage-1-introduction-to-behaviorist-ai) | Introduction to Behaviorist AI |
| [2](#stage-2-basics-of-reinforcement-learning) | Basics of Reinforcement Learning |
| [3](#stage-3-markov-decision-processes-mdps) | Markov Decision Processes (MDPs) |
| [4](#stage-4-rl-algorithms-and-techniques) | RL Algorithms and Techniques |
| [5](#stage-5-behaviorist-ai-in-robotics-and-games) | Behaviorist AI in Robotics and Games |
| [6](#stage-6-applications-and-use-cases-of-behaviorist-ai) | Applications and Use Cases of Behaviorist AI |
| [7](#stage-7-challenges-and-limitations-of-behaviorist-ai) | Challenges and Limitations of Behaviorist AI |

---

## Material

### Stage 1: Introduction to Behaviorist AI

- Definition
- Basic Process and Example
- Chapter Exercise

### Stage 2: Basics of Reinforcement Learning

- Reinforcement Learning (agent, environment, actions, rewards)
- Model-Based vs Model-Free
- Chapter Exercise

### Stage 3: Markov Decision Processes (MDPs)

- Markov Decision Process (1): States, Actions, Rewards
- Markov Decision Process (2): Probabilities, Policy, Value Function
- Bellman Equation
- Chapter Exercise

### Stage 4: RL Algorithms and Techniques

- Dynamic Programming (1)
- Dynamic Programming (2)
- Value Iteration
- Policy Iteration
- Reinforcement Learning Algorithms (overview)
- Value-Based (Q-Learning)
- Value-Based (Deep Q-Network, SARSA)
- Policy-Based (REINFORCE, Policy Gradient)
- Actor-Critic Algorithms
- On-Policy and Off-Policy Learning
- Chapter Exercise

### Stage 5: Behaviorist AI in Robotics and Games

- Behaviorist AI in Robotics (sensing, acting, and learning from feedback)
- Behaviorist AI in Games (game-playing agents)
- Chapter Exercise

### Stage 6: Applications and Use Cases of Behaviorist AI

- Applications and Usages of Behaviorist AI
- Examples of Applications in the Real World
- Chapter Exercise

### Stage 7: Challenges and Limitations of Behaviorist AI

- Challenges (for example reward design, exploration vs exploitation, data and computing cost)
- Limitations (for example safety, generalization, explainability)
- Chapter Exercise

---

