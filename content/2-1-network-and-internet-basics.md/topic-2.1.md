# Stage 1: What Is a Computer Network?

## Learning Goals

By the end of this stage, you will be able to:

1. Describe how data travels between connected devices using networks.
2. Define a computer network and explain how one works.
3. Explain the terms IP address, hostname, DNS, protocol, and bandwidth.
4. Describe the client-server and peer-to-peer network designs.
5. Give reasons why computers are networked.

**Topics covered:**

- Network overview
- Why computers are networked

---

# 1.1 Network Overview

## What Is a Computer Network?

### Explanation

A **computer network** is a group of **connected devices** that **share data and resources** with each other.

Let's define the words in that sentence:

- **Node**: Any device that is connected to a network, such as a laptop, a phone, a printer, or a server.
- **Resource**: Something that can be shared, such as a printer, a file, or an internet connection.
- **Server**: A computer that provides data or services to other devices on a network.

Devices can be connected in two ways:

| Connection | Meaning | Example |
|------------|---------|---------|
| **Wired** | Uses **cables** | An Ethernet cable between a laptop and a router |
| **Wireless** | Uses **radio waves** instead of cables | Wi-Fi |

Once devices are connected, they follow **protocols** to exchange data. A **protocol** is a set of agreed rules that devices follow so that they can understand each other, like two people agreeing to speak the same language. Examples of protocols:

| Protocol | Full name | What it is used for |
|----------|-----------|---------------------|
| **TCP/IP** | Transmission Control Protocol / Internet Protocol | The main rules for sending data across networks and the Internet |
| **SMTP** | Simple Mail Transfer Protocol | Sending email |
| **HTTP** | Hypertext Transfer Protocol | Loading web pages |

[insert image about several nodes (laptop, phone, printer, server) connected in a network]

### Worked Example

**Task:** Two laptops are connected with an Ethernet cable, and one sends a file to the other. Identify the parts of the network.

| Part | In this example |
|------|-----------------|
| Nodes | The two laptops |
| Connection | A wired connection (the Ethernet cable) |
| Resource shared | The file |
| Protocol | Rules such as TCP/IP that control how the file is sent |

### Activity

a. What is a node?
b. Name one wired and one wireless way of connecting devices.
c. What does HTTP help a computer do?

<details>
<summary><b>Answer</b></summary>

a. Any **device connected to a network**, such as a laptop, a phone, or a printer.
b. Wired: an **Ethernet cable**. Wireless: **Wi-Fi**.
c. **Load web pages.**

</details>

---

## The History and Size of Networks

### Explanation

The first example of a computer network was the **ARPANET** (Advanced Research Projects Agency Network). It was created in the **late 1960s** by **ARPA**, an agency of the U.S. Department of Defense. It was a **packet-switched** network, which means that data was broken into small pieces called **packets**, and each packet was sent separately and put back together at the other end.

[insert image about the early ARPANET with its nodes at universities and research centers]

Networks come in many sizes:

- **Very small**: Two laptops joined by an Ethernet cable.
- **Very large**: The **Internet**, which is a **global system of connected computer networks**.

Two common network sizes:

| Type | Full name | Area it covers | Example |
|------|-----------|----------------|---------|
| **LAN** | Local Area Network | A small area | A home, a school, or an office |
| **WAN** | Wide Area Network | A large area, such as cities or countries | The Internet |

### Worked Example

**Task:** Decide whether each network is a LAN or a WAN.

| Network | Type | Why |
|---------|------|-----|
| The computers in one classroom | LAN | Small area |
| A company linking its offices in three countries | WAN | Covers a large area |
| The Internet | WAN | Covers the whole world |

### Activity

a. Which network was the first example of a computer network?
b. What is a packet?
c. Is a home Wi-Fi network a LAN or a WAN?

<details>
<summary><b>Answer</b></summary>

a. The **ARPANET**, created in the late 1960s.
b. A **small piece of data** that is sent across a network and put back together at the destination.
c. A **LAN**.

</details>

---

## How Does a Computer Network Work?

### Explanation

A network works through a few simple ideas:

**1. Devices use IP addresses.**

An **IP address** (Internet Protocol address) is a **unique number** that identifies a device on a network, like a house address for a letter. An example looks like `192.168.1.25`.

**2. Hostnames and DNS make addresses easy to use.**

People find numbers hard to remember, so websites also have **hostnames**, which are names such as `www.example.com`. The **Domain Name System (DNS)** is a system of **DNS servers** that works like a phone book: it **looks up a hostname and gives back the matching IP address**, so devices can find each other.

**3. Protocols and algorithms control how data is sent.**

An **algorithm** is a step-by-step set of rules for doing a task. Protocols and algorithms together decide **how data is split up, sent, and put back together**.

**4. Networks follow standards.**

A **standard** is an agreed technical rule that lets equipment from different makers work together. Standards are set by organizations such as the **IEEE** (Institute of Electrical and Electronics Engineers):

| Standard | Used for |
|----------|----------|
| **Ethernet** | Wired networks |
| **802.11** | Wireless networks (Wi-Fi) |

[insert image about a DNS server turning a hostname into an IP address]

### Worked Example

**Task:** Follow what happens when you open a website by typing its name.

| Step | What happens |
|------|--------------|
| 1 | You type the hostname `www.example.com` into your browser |
| 2 | Your device asks a **DNS server**, "What is the IP address for this name?" |
| 3 | The DNS server replies with the **IP address** (for example, `192.0.2.10`) |
| 4 | Your device sends a request to that IP address using **HTTP** over **TCP/IP** |
| 5 | The server sends the web page back, as packets |
| 6 | Your browser puts the packets together and shows the page |

### Activity

a. What does DNS do?
b. What is the difference between a hostname and an IP address?
c. Which standard is used for Wi-Fi?
d. Who sets networking standards such as Ethernet and 802.11?

<details>
<summary><b>Answer</b></summary>

a. It **turns a hostname into an IP address**, so devices can find each other.
b. A **hostname** is a name that people can read (like `www.example.com`). An **IP address** is the number that devices use to find each other (like `192.0.2.10`).
c. **802.11**
d. Organizations such as the **IEEE**.

</details>

---

## Network Design (Architecture) and Bandwidth

### Explanation

**Network architecture** is the **physical and logical design** of a network, or how its parts are arranged and how they work together. There are two common designs:

| Design | How it works | Example |
|--------|--------------|---------|
| **Client-server** | **Clients** (devices that ask for things) request resources from a central **server** | A phone (client) asks a website's server for a web page |
| **Peer-to-peer (P2P)** | Every device is an equal, and the devices **share resources** like memory and processing power directly with each other | Friends sharing files directly between their computers |

[insert image about a client-server network next to a peer-to-peer network]

**Capacity**, also called **bandwidth**, measures **how much traffic (data) a network can handle** while still performing well. It is measured in **bits per second** (for example, **Mbps**, or megabits per second, where 1 megabit is one million bits). A higher bandwidth means more data can move at once.

### Worked Example

**Task 1:** A school computer asks the school's file server for a document. Which design is this?

**Client-server.** The computer is the client, and the file server is the central server that provides the document.

**Task 2:** How long does it take to send a 50 MB file over a 100 Mbps connection? (1 byte = 8 bits, so 1 MB = 8 megabits.)

1. File size in megabits: 50 × 8 = **400 megabits**
2. Time = 400 ÷ 100 = **4 seconds** (in the best case; real speeds are usually a little slower)

### Activity

a. In a client-server network, what does the client do?
b. In which design do devices share resources directly with each other?
c. How long does a 25 MB file take to send over a 100 Mbps connection? (Hint: 25 × 8 = 200 megabits.)

<details>
<summary><b>Answer</b></summary>

a. It **requests resources** from the server.
b. **Peer-to-peer (P2P)**.
c. 200 ÷ 100 = **2 seconds**.

</details>

---

# 1.2 Why Computers Are Networked

## Explanation

Computer networks make it possible to **share information quickly** and to **use resources efficiently**. Here are the main reasons why computers are networked:

| Benefit | What it means | Example |
|---------|---------------|---------|
| **Resource sharing** | Many devices share the same resources, such as printers, files, scanners, and photocopiers. This is helpful for large organizations that are spread out around the world, because they can use one network to connect all their employees. | An office where 20 people print on one shared printer |
| **Flexibility** | People can choose the communication and sharing method that suits them. | Using email, instant messaging, or an app like WhatsApp |
| **Higher connectivity** | People can stay connected **wherever they are**. Video calling and document-sharing apps let workers **collaborate** (work together) from a distance. | Zoom meetings and Google Docs |
| **Data security and management** | Data is **centralized** (kept in one main place) on shared servers. **Network administrators** (the people who run the network) can manage and protect the data more easily, make regular **backups** (extra copies), and apply security measures to all devices at once, such as **multi-factor authentication** (checking identity with more than one proof, like a password plus a phone code). | A company backing up all its files every night from one server |
| **Storage capacity** | Organizations grow and have more and more data. Networks, especially ones using **cloud technology** (storage and services provided over the Internet), can store huge amounts of data and backups on a central remote server that everyone can reach at any time. | Saving files to a cloud drive |
| **Entertainment** | Networks, especially the Internet, provide games, streaming music, and videos. Multiplayer games need a **LAN** or a **WAN** (such as the Internet) to work. | Playing an online game with friends |

[insert image about the benefits of networks: sharing a printer, video calls, cloud storage, and online gaming]

## Worked Example

**Task 1:** An office has 10 employees who all need to print. A printer costs $300. Compare buying one printer for each person with sharing one printer over a network.

| Option | Number of printers | Total cost |
|--------|--------------------|------------|
| No network (one printer each) | 10 | 10 × $300 = **$3,000** |
| Network (one shared printer) | 1 | **$300** |

The network saves **$2,700**. This is the benefit of **resource sharing**.

**Task 2:** Match each situation to a benefit of networking.

| Situation | Benefit |
|-----------|---------|
| A team edits the same document from different cities | Higher connectivity |
| A company backs up everything from one server | Data security and management |
| A student saves a large project in the cloud | Storage capacity |
| Friends play an online match together | Entertainment |

## Activity

Name the benefit of networking in each case:

a. A school has one scanner that all teachers use.
b. An IT manager turns on multi-factor authentication for every computer at once.
c. A worker joins a video call from home.
d. A person can choose to message a friend with email or with WhatsApp.

<details>
<summary><b>Answer</b></summary>

a. **Resource sharing**
b. **Data security and management**
c. **Higher connectivity**
d. **Flexibility**

</details>

---

## Stage 1 Summary

- A **computer network** is a group of connected **nodes** (devices) that share data and resources, using **wired** or **wireless** connections and **protocols** such as TCP/IP, SMTP, and HTTP.
- The **ARPANET** (late 1960s) was the first example of a computer network. The **Internet** is a global system of connected networks.
- A **LAN** covers a small area, and a **WAN** covers a large area.
- Devices find each other with **IP addresses**. **DNS** looks up a **hostname** and gives back its IP address.
- Networks follow **standards**, such as **Ethernet** (wired) and **802.11** (wireless), set by organizations like the **IEEE**.
- **Architecture** is the network's design. In **client-server**, clients request resources from a central server. In **peer-to-peer (P2P)**, devices share resources directly.
- **Bandwidth** shows how much traffic a network can handle, measured in bits per second.
- Computers are networked for **resource sharing**, **flexibility**, **higher connectivity**, **data security and management**, **storage capacity**, and **entertainment**.

# Stage 2: Network Fundamentals

## Learning Goals

By the end of this stage, you will be able to:

1. Describe how data travels between connected devices using networks.
2. Identify common network devices and explain what each one does.
3. Compare wired and wireless media.
4. Tell the difference between types of networks, such as LAN and WAN.
5. Describe star and mesh layouts (topologies).
6. Explain basic Internet ideas: TCP/IP, IP addresses, domain names, the Web, and URLs.

**Topics covered:**

- Devices (Computers, Server, Switch, Router, Modem, Access Point)
- Media (Wired, Wireless)
- Types of network (LAN, WAN)
- Layouts (Topologies: Star, Mesh)
- Internet fundamentals and other key Internet concepts

---

# 2.1 Devices

## Explanation

A computer network is built from parts that work together. The basic building blocks are:

| Component | What it is |
|-----------|------------|
| **Node** | Any device connected to the network, such as a computer, printer, or smartphone |
| **Link** | The **communication channel** that connects devices (cables, fiber optics, or wireless signals) |
| **Protocol** | The **set of rules** that decides how data is sent over the network |
| **Network Interface Card (NIC)** | A hardware part that **connects a computer to a network**. Every device that joins a network needs one (often built in). |

Here are the main network devices:

| Device | What it does | Easy way to think of it |
|--------|--------------|-------------------------|
| **Computer** | An **end device** where people use the network (laptops, phones, desktops) | The people at the party |
| **Server** | A computer that **provides data or services** to other devices, such as web pages or files | The kitchen that serves everyone |
| **Switch** | **Connects devices inside one network** and sends data **only to the device it is meant for** | A mail clerk who delivers each letter to the right desk |
| **Router** | **Directs traffic between different networks**, such as your home LAN and the Internet | A road junction that sends traffic toward the right city |
| **Modem** | **Converts** digital data into a signal that can travel over a phone, cable, or fiber line, and **converts it back** at the other end | A translator between your network and your Internet line |
| **Access Point (AP)** | Lets **wireless devices** connect to a **wired network** using Wi-Fi | A doorway between cables and Wi-Fi |

Some other devices you may meet:

| Device | What it does |
|--------|--------------|
| **Hub** | A basic device that **sends data to every connected device**, whether they need it or not (a switch is smarter because it sends data only to the right device) |
| **Firewall** | A security device that **monitors and filters** incoming and outgoing traffic using security rules |
| **Gateway** | An **entrance to another network**. It can **translate** between networks that use different protocols. |
| **Repeater** | **Boosts or regenerates a signal** so it can travel farther |

*(In many homes, one box combines a modem, a router, a switch, and an access point.)*

[insert image about a network diagram with a modem, router, switch, access point, server, and several computers]

## Worked Example

**Task:** Follow a laptop's request for a web page through a home network.

| Step | Device | What happens |
|------|--------|--------------|
| 1 | Laptop (NIC) | The laptop's NIC sends the request |
| 2 | Access point | The request travels over Wi-Fi to the access point, which passes it to the wired network |
| 3 | Switch | The switch sends it to the router, and only to the router |
| 4 | Router | The router sends it out toward the Internet |
| 5 | Modem | The modem converts the data into a signal for the Internet line |
| 6 | ISP and Internet | The request reaches the web server, which sends the page back along the same path |

## Activity

Name the device for each job:

a. Sends data only to the intended device inside one network.
b. Directs traffic between your home network and the Internet.
c. Lets a phone connect to a wired network using Wi-Fi.
d. Provides web pages to other devices.
e. Sends data to every device, whether needed or not.

<details>
<summary><b>Answer</b></summary>

a. **Switch**
b. **Router**
c. **Access point**
d. **Server**
e. **Hub**

</details>

---

# 2.2 Media

## Explanation

**Network media** (the plural of *medium*) are the **paths that carry data** between devices. These are the **links** of a network. There are two groups: **wired** and **wireless**.

**Wired media** use physical cables:

- **Ethernet cable (twisted-pair copper)**: The common cable for LANs. Data travels as **electrical signals**.
- **Fiber-optic cable**: Thin strands of glass. Data travels as **pulses of light**, which can carry a lot of data over long distances.

**Wireless media** use **radio waves** (or other signals) through the air instead of cables. The most common example is **Wi-Fi**.

| Feature | Wired | Wireless |
|---------|-------|----------|
| Speed | Usually fast and steady | Often slower, and can change |
| Reliability | High, less affected by interference | Can be affected by walls, distance, and other signals |
| Movement | Devices must stay near the cable | Devices can move freely |
| Setup | Needs cables | Easy, no cables |
| Security | Harder to tap into | Needs protection such as a password and encryption |

**Interference** means other signals or objects that disturb a signal and make it weaker.

[insert image about an Ethernet cable, a fiber-optic cable, and a Wi-Fi signal]

## Worked Example

**Task:** Choose the best medium.

| Situation | Best medium | Why |
|-----------|-------------|-----|
| A desktop computer in a gaming room that needs steady, fast speed | Ethernet cable | Fast and reliable |
| A phone and tablet moving around the house | Wi-Fi | Devices can move freely |
| A link carrying huge amounts of data between two buildings far apart | Fiber-optic cable | Light signals carry a lot of data over long distances |

## Activity

a. Which wired medium sends data as pulses of light?
b. Give one advantage of wireless media and one of wired media.
c. What is a link in a network?

<details>
<summary><b>Answer</b></summary>

a. **Fiber-optic cable**
b. Wireless: devices can **move freely** and there are **no cables**. Wired: usually **faster and more reliable**.
c. The **communication channel** that connects devices, such as a cable, a fiber, or a wireless signal.

</details>

---

# 2.3 Types of Network

## Explanation

Networks are grouped by **how large an area they cover** and **who can use them**.

| Type | Full name | What it is | Example |
|------|-----------|------------|---------|
| **LAN** | Local Area Network | Covers a **small area**, such as an office or a home. Devices share resources like printers and files. | Your home Wi-Fi network |
| **WAN** | Wide Area Network | Covers a **large area**, such as cities or countries. The **Internet** is the largest WAN. | A company linking offices in different countries |
| **MAN** | Metropolitan Area Network | Spans **a city**. It is bigger than a LAN but smaller than a WAN. | A network connecting a city's libraries and offices |
| **VPN** | Virtual Private Network | Creates a **secure, encrypted connection** over a less secure network like the Internet. It is often used to reach a workplace's systems from far away. | An employee working from home who connects safely to the office network |
| **Intranet** | | A **private network** that only an organization's **staff** can use, for internal communication and resources | A company's internal website for employees |
| **Extranet** | | A controlled private network that gives **limited access to outsiders**, such as suppliers or partners, through a **secure login** | A supplier portal where partners track orders |

*(Encrypted means the data is scrambled so that only approved people can read it.)*

[insert image about the sizes of networks: LAN, MAN, and WAN]

## Worked Example

**Task:** Decide which network type fits each situation.

| Situation | Type | Why |
|-----------|------|-----|
| The computers in one school building | LAN | Small area |
| A university network joining campuses across a city | MAN | Spans a city |
| The global Internet | WAN | Covers the whole world |
| An employee safely reaching the company's files from a cafe | VPN | Secure connection over the Internet |

## Activity

a. What is the difference between a LAN and a WAN?
b. Which network lets only a company's own staff use its internal website?
c. Which network type gives suppliers limited, secure access?

<details>
<summary><b>Answer</b></summary>

a. A **LAN** covers a **small area** (like a home or office). A **WAN** covers a **large area** (like cities or countries).
b. An **intranet**
c. An **extranet**

</details>

---

# 2.4 Layouts (Topologies)

## Explanation

A **topology** is the **layout** of a network: how its devices are arranged and connected. Two common layouts are **star** and **mesh**.

### Star Topology

In a **star**, every device connects to **one central device**, usually a **switch**. The shape looks like a star.

| Advantages | Disadvantages |
|------------|---------------|
| Easy to add or remove a device | If the **central device fails**, the **whole network stops** |
| If one device or cable fails, the **others keep working** | Needs a lot of cable to the center |

### Mesh Topology

In a **mesh**, devices are connected to **many other devices**. In a **full mesh**, **every device connects to every other device**.

| Advantages | Disadvantages |
|------------|---------------|
| Very **reliable**: if one link fails, data can take another path | **Expensive** and complicated, because it needs many links |
| Data has many possible routes | Harder to set up and manage |

[insert image about a star topology and a mesh topology]

## Worked Example

**Task:** Compare the number of links needed to connect devices.

- **Star** with *n* devices: each device has one link to the center, so **n links**.
- **Full mesh** with *n* devices: every pair of devices has a link, so **n × (n − 1) ÷ 2 links**.

| Number of devices | Star links | Full mesh links |
|-------------------|------------|-----------------|
| 5 | 5 | 5 × 4 ÷ 2 = **10** |
| 10 | 10 | 10 × 9 ÷ 2 = **45** |

A full mesh needs many more links as the network grows, which is why it costs more.

## Activity

a. In a star network, what happens if one computer's cable breaks?
b. In a star network, what happens if the central switch fails?
c. How many links does a full mesh of 6 devices need?
d. Which layout is more reliable, star or mesh?

<details>
<summary><b>Answer</b></summary>

a. Only that computer loses its connection. The **others keep working**.
b. The **whole network stops**.
c. 6 × 5 ÷ 2 = **15 links**
d. **Mesh**, because data can take another path if a link fails.

</details>

---

# Stage 3: Internet Fundamentals

**Topics covered:**

- Internet vs the web
- TCP/IP
- IP addresses
- Domain names and DNS
- URL parts and from click to page

---

# 3.1 Internet Fundamentals and Other Key Concepts

## TCP/IP and IP Addresses

### Explanation

**TCP/IP** (Transmission Control Protocol / Internet Protocol) is the **group of protocols used to connect devices on the Internet**. It controls how data is **broken into packets** (small pieces), **sent**, and **put back together**.

- **TCP**: Makes sure data arrives **reliably, in the right order, and without errors**.
- **IP**: Handles **addressing and routing** (choosing the path), so that each packet reaches the **correct destination**.

An **IP address** is a unique number for a device on a network. There are two versions:

| Version | Address size | How many addresses |
|---------|--------------|--------------------|
| **IPv4** | **32 bits** | 2³² = 4,294,967,296 (about 4.3 billion) |
| **IPv6** | **128 bits** | 2¹²⁸, an enormously larger number |

IPv6 was created because the world was running out of IPv4 addresses.

[insert image about data being split into packets by TCP and routed to a destination by IP]

### Worked Example

**Task:** A file is sent from one computer to another.

| Step | Protocol | What happens |
|------|----------|--------------|
| 1 | TCP | Breaks the file into packets and numbers them |
| 2 | IP | Adds the destination IP address and sends each packet along a route |
| 3 | IP | The packets may take different routes across the network |
| 4 | TCP | At the destination, puts the packets back in order and asks for any missing ones to be sent again |

### Activity

a. Which protocol checks that data arrives in the correct order?
b. How many bits is an IPv4 address? An IPv6 address?

<details>
<summary><b>Answer</b></summary>

a. **TCP**
b. IPv4: **32 bits**. IPv6: **128 bits**.

</details>

---

## Domain Names and DNS

### Explanation

A **domain name** is a **human-readable address** for a website, such as `www.example.com`. It is **mapped to the website's IP address** by the **Domain Name System (DNS)**, which **translates domain names into IP addresses** so that browsers can load Internet resources.

Parts of a domain name:

| Part | Meaning | Example |
|------|---------|---------|
| **Top-Level Domain (TLD)** | The **last part** of the domain name | `.com`, `.org`, `.net` |
| **Domain** | The main name of the site | `example` |
| **Subdomain** | A part that goes **before** the domain, often used to organize sections of a website | `mail` in `mail.example.com` |

### Worked Example

**Task:** Break down `blog.example.org`.

| Part | Value |
|------|-------|
| Subdomain | `blog` |
| Domain | `example` |
| TLD | `.org` |

### Activity

Identify the TLD and the subdomain in `shop.mystore.com`.

<details>
<summary><b>Answer</b></summary>

TLD: **.com**. Subdomain: **shop**.

</details>

---

## The World Wide Web, HTTP/HTTPS, and URLs

### Explanation

The **World Wide Web** (the **Web**) is a system of **linked documents and media** that you reach over the Internet with a **web browser**. The Web is one service that runs on the Internet. The Internet is the network itself.

- **HTTP** (HyperText Transfer Protocol): The foundation of data exchange on the Web.
- **HTTPS** (HTTP Secure): The same, but with a layer of **encryption** added, so the communication is secure.
- **URL** (Uniform Resource Locator): The **unique address of a resource on the Web**. It tells the browser the **protocol**, the **domain**, and the **path** to the exact page.

### Worked Example

**Task:** Break down the URL `https://www.example.com/news/today.html`.

| Part | Value | Meaning |
|------|-------|---------|
| Protocol | `https` | Use secure HTTP |
| Domain | `www.example.com` | The website's name |
| Path | `/news/today.html` | The exact page on that site |

### Activity

a. What does the "S" in HTTPS add?
b. Name the three parts of a URL described above.

<details>
<summary><b>Answer</b></summary>

a. **Encryption** (secure communication).
b. The **protocol**, the **domain**, and the **path**.

</details>

---

## Other Key Internet Concepts

### Explanation

| Term | Meaning |
|------|---------|
| **Internet Service Provider (ISP)** | A company that **provides access to the Internet** |
| **Latency** | The **delay** before data starts to transfer after you ask for it |
| **FTP (File Transfer Protocol)** | A protocol for **moving files between computers** on a network |
| **SMTP** | The protocol for **sending** email |
| **POP3 (Post Office Protocol)** | A protocol for **receiving** email by downloading it to your device |
| **IMAP (Internet Message Access Protocol)** | A protocol for **receiving** email while keeping it on the mail server |

### Worked Example

**Task:** Name the correct term.

| Situation | Term |
|-----------|------|
| A pause between clicking a link and the page starting to load | Latency |
| The company whose service you pay for to get online | ISP |
| Uploading website files to a server | FTP |

### Activity

a. Which protocol is used to send email?
b. What is latency?

<details>
<summary><b>Answer</b></summary>

a. **SMTP**
b. The **delay** before data transfer begins after an instruction.

</details>

---

## Stage 2 and 3 Summary

- **Nodes** are devices on the network. **Links** connect them, **protocols** are the rules, and a **NIC** connects a computer to the network.
- A **switch** connects devices inside one network, a **router** connects different networks, a **modem** converts signals for the Internet line, and an **access point** adds Wi-Fi to a wired network. A **server** provides services.
- **Wired** media (Ethernet, fiber-optic) are fast and reliable. **Wireless** media (Wi-Fi) let devices move freely.
- A **LAN** covers a small area, a **MAN** a city, and a **WAN** a large area. A **VPN** is a secure connection, an **intranet** is for staff only, and an **extranet** gives limited access to outsiders.
- A **star** topology uses one central device, and a **mesh** topology connects many devices to each other for greater reliability.
- **TCP/IP** breaks data into packets and delivers them. **DNS** turns domain names into IP addresses. The **Web** uses **HTTP/HTTPS** and **URLs**.
