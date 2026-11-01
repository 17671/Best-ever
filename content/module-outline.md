# PikaByte — Module Topics Outline

# Hardware, Networks & Behavorist AI — Module Outline

## Concise Plan & Status

This section provides a quick overview of the module's 8 chapters and their current development status.

| Part | Chapter | Filename | Status |
| :--- | :--- | :--- | :--- |
| **Part 1: Hardware & Data** | 1.1 Number Systems and Data | `1-1-number-systems-and-data.md` | Outline only |
| | 1.2 Hardware & Von Neumann Model | `1-2-hardware-and-von-neumann.md` | Outline only |
| **Part 2: Networks & Security** | 2.1 Network & Internet Basics | `2-1-network-and-internet-basics.md` | Outline only |
| | 2.2 Network Security | `2-2-network-security.md` | Outline only |
| **Part 3: Behaviorist AI** | 3.1 Intro to Behaviorist AI & RL | `3-1-intro-to-behaviorist-ai.md` | Outline only |
| | 3.2 RL Algorithms and MDPs | `3-2-rl-algorithms-and-mdps.md` | Outline only |
| | 3.3 AI in Robotics and Games | `3-3-ai-in-robotics-and-games.md` | Outline only |
| | 3.4 AI Challenges and Limitations | `3-4-ai-challenges-and-limitations.md` | Outline only |

---

## Part 2: Chapters Breakdown & Learning Goals

### Part 1: Hardware & Data

#### Chapter 1.1: Number Systems and Data (`1-1-number-systems-and-data.md`)
**Chapter Overview**
This chapter introduces what a computer is and how it works, from the basic workflow of input, processing, storage, and output down to the binary data it uses. You'll study number systems and data storage.

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Define a computer, describe its basic workflow, and distinguish between types of computers.
- Convert between binary, decimal, and hexadecimal number systems.
- Explain how numbers, text, images, audio, and video are stored as binary data.
- Distinguish between primary (RAM) and secondary storage (SSD/HDD).

**Material**
- Stage 1: Computers and Data
    - Definition of a Computer
    - The Basic Workflow of a Computer (input, processing, storage, output)
    - Different Types of Computers
- Stage 2: Number Systems
    - Number System Overview
    - Binary Number System
    - Decimal to Binary and Binary to Decimal
    - Hexadecimal to Binary and Binary to Hexadecimal
    - Hexadecimal to Decimal and Decimal to Hexadecimal
- Stage 3: Data Storage
    - Definition
    - How Does Data Storage Work
    - Representing Data in Binary (numbers, text, images, audio, video)
    - Types of Data Storage (primary and secondary)
    - Data Storage Devices (HDD, SSD, USB drives)
- Stage 4: Chapter Exercise

#### Chapter 1.2: Hardware and the Von Neumann Model (`1-2-hardware-and-von-neumann.md`)
**Chapter Overview**
This chapter covers the physical components of a computer and how they execute instructions using the Von Neumann model. It covers the physical components that make up a computer and how a program runs.

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Describe the Von Neumann model and its main components.
- Identify input, output, and internal hardware components, and explain the difference between internal and external hardware.
- Explain how hardware components work together to execute a program.

**Material**
- Stage 1: Von Neumann Model
    - Definition
    - Process (fetch-decode-execute)
    - Components (1): CPU (control unit and ALU)
    - Components (2): Memory, Input, and Output
- Stage 2: Computer Hardware
    - Hardware Definition
    - Input Devices: Mouse, Keyboard, Microphone, Camera, Touchpad
    - Output Devices: Monitor, Printer, Speaker
    - Internal Hardware: Motherboard, CPU, RAM, RAM vs ROM, Graphics Card, Power Supply
    - Ports and External Storage: USB, Memory Card
- Stage 3: Program Execution
    - Definition
    - How Program Execution Works (from stored program to running task)
- Stage 4: Chapter Exercise

---

### Part 2: Networks & Security

#### Chapter 2.1: Network and Internet Basics (`2-1-network-and-internet-basics.md`)
**Chapter Overview**
A computer network connects two or more computers so they can share data and resources. This chapter covers the parts of a network, the types of network, and how the internet works.

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Define a computer network and explain why computers are networked.
- Identify the common parts of a network and describe what each does.
- Distinguish between LAN and WAN.
- Explain how the internet delivers data using TCP/IP, IP addresses, and domain names.

**Material**
- Stage 1: What Is a Computer Network?
    - Network overview
    - Why computers are networked
- Stage 2: Network Fundamentals
    - Devices (Computers, Server, Switch, Router, Modem, Access point)
    - Media (Wired, Wireless)
    - Types of network (LAN, WAN)
    - Layouts (Topologies: Star, Mesh)
- Stage 3: Internet Fundamentals
    - Internet vs the web
    - TCP/IP
    - IP addresses
    - Domain names and DNS
    - URL parts and from click to page
- Stage 4: Chapter Exercise

#### Chapter 2.2: Network Security (`2-2-network-security.md`)
**Chapter Overview**
This chapter covers network security, explaining why it matters and how data is protected as it travels across the internet.

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Explain privacy, authentication, integrity, and nonrepudiation.
- Match common protections to each security goal.

**Material**
- Stage 1: Security in Networks
    - Why it matters
    - Privacy (confidentiality)
    - Authentication
    - Integrity
    - Nonrepudiation
    - Common protections (Firewall, Encryption)
- Stage 2: Chapter Exercise

---

### Part 3: Behaviorist AI

#### Chapter 3.1: Intro to Behaviorist AI & RL (`3-1-intro-to-behaviorist-ai.md`)
**Chapter Overview**
This chapter explains how an AI system can learn behavior from experience. You'll start with what Behaviorist AI is and the basics of reinforcement learning (RL).

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Define Behaviorist AI and describe its basic process with an example.
- Explain reinforcement learning in terms of agent, environment, actions, and rewards.
- Distinguish model-based from model-free learning.

**Material**
- Stage 1: Introduction to Behaviorist AI
    - Definition
    - Basic Process and Example
- Stage 2: Basics of Reinforcement Learning
    - Reinforcement Learning (agent, environment, actions, rewards)
    - Model-Based vs Model-Free
- Stage 3: Chapter Exercise

#### Chapter 3.2: RL Algorithms and MDPs (`3-2-rl-algorithms-and-mdps.md`)
**Chapter Overview**
This chapter introduces Markov Decision Processes (MDPs) and the algorithms built on them to calculate the best decisions.

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Describe the parts of an MDP (states, actions, rewards, policy).
- Explain Q-learning conceptually.
- Understand the balance between exploration and exploitation.

**Material**
- Stage 1: Markov Decision Processes (MDPs)
    - Markov Decision Process (1): States, Actions, Rewards
    - Markov Decision Process (2): Policy
- Stage 2: RL Algorithms and Techniques
    - Reinforcement Learning Algorithms (overview)
    - Value-Based (Q-Learning conceptual overview)
    - Exploration vs. Exploitation
- Stage 3: Chapter Exercise

#### Chapter 3.3: AI in Robotics and Games (`3-3-ai-in-robotics-and-games.md`)
**Chapter Overview**
This chapter covers how these methods are used in robotics and games, and looks at real-world applications.

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Describe how RL is used in robotics and games.
- Give examples of real-world applications of Behaviorist AI.

**Material**
- Stage 1: Behaviorist AI in Robotics and Games
    - Behaviorist AI in Robotics (sensing, acting, and learning from feedback)
    - Behaviorist AI in Games (game-playing agents)
- Stage 2: Applications and Use Cases of Behaviorist AI
    - Applications and Usages of Behaviorist AI
    - Examples of Applications in the Real World
- Stage 3: Chapter Exercise

#### Chapter 3.4: AI Challenges and Limitations (`3-4-ai-challenges-and-limitations.md`)
**Chapter Overview**
This final chapter examines the challenges and limitations of the approach.

**Learning Outcomes**
By the end of this chapter, you will be able to:
- Identify the main challenges of Behaviorist AI.
- Describe the limitations of the technology.

**Material**
- Stage 1: Challenges and Limitations of Behaviorist AI
    - Challenges (reward design, exploration vs exploitation, data and computing cost)
    - Limitations (safety, generalization, explainability)
- Stage 2: Chapter Exercise
## References for Research

- [Cisco Networking Academy](https://www.netacad.com/)
- [NVIDIA AI Resources](https://www.nvidia.com/en-us/ai/)
- [Google Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course)
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework)


> [!IMPORTANT]
> These seven topics form the initial learning outline. The team should research and verify the information before completing the final learning materials. At least one selected topic should be developed into a complete beginner-friendly learning section with explanations, visuals, activities, answers, and references.
