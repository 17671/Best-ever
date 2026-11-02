# Stage 1: Computers and Data

## Learning Goals

By the end of this stage, you will be able to:

1. Identify the core physical components of a computer and explain their basic functions.

**Topics covered:**

- Definition of a Computer
- The Basic Workflow of a Computer (input, processing, storage, output)
- Different Types of Computers

---

# 1.1 Definition of a Computer

## Explanation

A **computer** is an electronic machine that takes in **data**, works on it by following a list of **instructions**, and gives back a result.

Let's define the words we just used:

- **Data**: Raw information a computer can work with, such as numbers, text, pictures, or sound.
- **Instruction**: A single step that tells the computer what to do (for example, "add these two numbers").
- **Program**: A complete list of instructions that tells the computer how to finish a task.

Every computer does four basic jobs:

| # | Function | What it means | Example |
|---|----------|---------------|---------|
| 1 | **Input** | Receives data from the outside world | Typing on a keyboard, moving a mouse |
| 2 | **Processing** | Works on the data using the program's instructions | Adding numbers, comparing two values |
| 3 | **Output** | Sends the finished result back to the user | Showing text on a screen, printing a page |
| 4 | **Storage** | Saves data so it can be used later | Saving a file to a hard drive |

Computers come in many forms. A **personal computer (PC)** is a computer made for one person to use, like a desktop or laptop. A **smartphone** is a pocket-sized computer that also works as a phone. A **supercomputer** is an extremely powerful computer used for huge tasks such as scientific research.

[insert image about the four basic functions of a computer: input, processing, output, storage]

## Worked Example

**Task:** You use a calculator app on your phone to add 5 + 3.

| Step | What happens | Function |
|------|--------------|----------|
| 1 | You tap `5`, `+`, `3` on the touchscreen | Input |
| 2 | The phone adds the numbers and gets 8 | Processing |
| 3 | The phone shows `8` on the screen | Output |
| 4 | The phone keeps the answer in its history list | Storage |

## Activity

You take a photo with your phone and save it to the gallery. Which of the four basic functions is happening in each step?

a. The camera captures the picture.
b. The phone turns the picture into a file it can handle.
c. The picture appears on your screen as a preview.
d. The photo is kept in the gallery.

<details>
<summary><b>Answer</b></summary>

a. **Input**: the camera gathers data from the outside world.
b. **Processing**: the phone works on the data.
c. **Output**: the result is shown to the user.
d. **Storage**: the data is saved for later use.

</details>

---

## 1.1.1 Turing Model

### Explanation

In 1936, a mathematician named **Alan Turing** proposed the idea of a machine that could do *any* calculation, as long as it was given the right instructions. This idea is called the **Turing Machine**.

A **Turing Machine** is an imaginary (hypothetical) device with three parts:

- A very long **tape** (it never ends) where symbols are written and read.
- A **head** that reads and writes symbols on the tape.
- A set of **rules** that tell the head what to do next, based on the symbol it sees.

[insert image about a Turing Machine with its tape and head]

From this idea comes the **Turing model**, which describes a computer as a **programmable data processor**. *Programmable* means you can change what the computer does by changing its program. The computer is treated like a **black box**: a device where you only see what goes in and what comes out, not what happens inside.

[insert image about a black box diagram: Input data -> Computer -> Output data]

In this model, the output depends on **two things**: the **input data** and the **program**. Changing either one can change the result. But running the *same program* with the *same input* always gives the *same output*.

> **Note:** This model is a little too broad. Even a simple calculator fits this description, but we don't usually call a calculator a full computer.

Turing's work also showed that any problem that *can* be solved by following steps can be solved by a computer, as long as it has the correct program.

### Worked Example

The input data is always `3, 12, 8, 22`. Watch how the output changes when only the program changes.

| Program | Input data | Output data |
|---------|------------|-------------|
| Sort (put in order, smallest first) | 3, 12, 8, 22 | 3, 8, 12, 22 |
| Add (find the total) | 3, 12, 8, 22 | 45 |
| Find smallest | 3, 12, 8, 22 | 3 |

[insert image about one computer running three different programs (Sort, Add, Find smallest) on the same input]

### Activity

Your input data is `5, 2, 9`. What is the output for each program?

a. Sort
b. Add
c. Find smallest

<details>
<summary><b>Answer</b></summary>

a. **Sort** gives `2, 5, 9`
b. **Add** gives `16` (5 + 2 + 9)
c. **Find smallest** gives `2`

The input stayed the same, but the program changed the output.

</details>

---

## 1.1.2 von Neumann Model

### Explanation

Around 1944–1945, a mathematician named **John von Neumann** added a new idea to Turing's work. He pointed out that **programs and data are both just information**, so a computer can keep *both* in its **memory**.

**Memory** is the part of the computer that holds programs and data while the computer is working. Before this idea, early computers had to be rewired by hand every time they needed to do a new job. With the von Neumann model, switching tasks is as easy as loading a different program.

The **von Neumann model** splits a computer into four parts, called **subsystems**:

| Subsystem | What it does |
|-----------|--------------|
| **Memory** | Stores both programs and data |
| **Arithmetic Logic Unit (ALU)** | Does the math (like adding) and the logic (like comparing two numbers) |
| **Control Unit** | Manages and directs all the other parts, like a traffic controller |
| **Input/Output** | Moves data between the computer and the outside world |

The control unit repeats a simple cycle: it **fetches** (gets) an instruction from memory, then **executes** (carries out) it, then moves on to the next one. This keeps programs running in an orderly and predictable way.

[insert image about the von Neumann model showing Memory, ALU, Control Unit, and Input/Output]

### Worked Example

**Task:** Add two numbers, 4 and 6.

| Step | Subsystem | What it does |
|------|-----------|--------------|
| 1 | Input/Output | Receives the numbers 4 and 6 from the keyboard |
| 2 | Memory | Stores 4 and 6, along with the "add" instruction |
| 3 | Control Unit | Fetches the "add" instruction from memory |
| 4 | ALU | Calculates 4 + 6 = 10 |
| 5 | Input/Output | Sends 10 to the screen |

### Activity

Match each job to the correct subsystem: **Memory**, **ALU**, **Control Unit**, or **Input/Output**.

a. Checking whether 15 is bigger than 12
b. Holding a program while it runs
c. Showing a result on the monitor
d. Deciding which instruction runs next

<details>
<summary><b>Answer</b></summary>

a. **ALU** (comparing is a logic operation)
b. **Memory**
c. **Input/Output**
d. **Control Unit**

</details>

---

## 1.1.3 Computer Components

### Explanation

A computer is made of three main components:

- **Hardware**: The physical parts of the computer that you can touch.
- **Software**: The programs and instructions stored in the computer's memory.
- **Data**: Information the computer can read, change, or store.

**Hardware** includes memory, the ALU, and the input/output parts. **Input** means the data or commands the computer receives from users or devices. **Output** means the result the computer gives back (such as a display or a printout). Together, they let the user and the computer communicate.

[insert image about input example (keyboard to computer) and output example (computer to printer)]

Computers store and process data in **binary**, a number system that uses only two digits: `0` and `1`. Numbers, text, pictures, and sound must all be converted into binary before a computer can work with them. **Software** is what lets the hardware and the data work together, because it tells the hardware how to handle the data.

Software has four key parts:

1. **Stored programs**: Modern computers keep both programs and data in memory. Early computers needed to be set up by hand for each task.

   [insert image about memory split into a Program section and a Data section]

2. **Sequence of instructions**: A program is a series of instructions that work on data. The same instructions can be reused and rearranged to build different programs.

   [insert image about a four-step instruction list: input first number, input second number, add and store, output result]

3. **Algorithms**: An **algorithm** is a step-by-step set of rules for solving a problem. Programmers plan an algorithm *before* they write a program.

   [insert image about an algorithm flowchart: Input -> Set of rules -> Output]

4. **Languages**: Early computers only understood **machine language**, which is written entirely in binary. Later, **symbolic languages** were created, which use letters and symbols so people can write programs more easily. One early standard is **ASCII** (explained in section 1.2.2).

### Worked Example

**Task:** Describe the sequence of instructions for adding two numbers.

1. Input the first number into memory.
2. Input the second number into memory.
3. Add the two numbers and store the result in memory.
4. Output the result.

These steps are also a small **algorithm**: a clear, step-by-step way to solve the problem of adding two numbers.

### Activity

Write a short algorithm (3 to 5 steps) for finding the **average** of two numbers. (The average is the total of the numbers divided by how many numbers there are.)

<details>
<summary><b>Answer</b></summary>

One possible answer:

1. Input the first number into memory.
2. Input the second number into memory.
3. Add the two numbers together.
4. Divide the total by 2 and store the result in memory.
5. Output the result.

Any answer with clear, ordered steps that gives the right result is correct.

</details>

---

# 1.2 The Basic Workflow of a Computer

A **workflow** is the path that data follows from start to finish. In a computer, data moves through four stages:

**Input → Processing → Storage → Output**

[insert image about the computer workflow: input, processing, storage, output]

---

## 1.2.1 Input

### Explanation

For a computer to produce any **output**, it first has to receive **input** to work on. An **input system** has four elements:

1. **Input interface**: The part that collects data from outside and delivers it to the computer. It includes:
   - **Human Interface Devices (HID)**: Devices people use to talk to the computer, such as keyboards, mice, and touchscreens.
   - **Input/Output ports**: Physical connection points, such as USB ports, audio jacks, and HDMI ports, where devices plug in.
2. **Input controllers**: Small circuits that receive signals from input devices, prepare the data, and pass it to the **central processing unit (CPU)**. (The CPU is the "brain" of the computer. More on it in 1.2.2.)

   [insert image about an input/output controller device]

3. **Input devices**: Tools that users interact with to give data to the computer. Each one handles a specific kind of data:

   | Device | What it does |
   |--------|--------------|
   | **Keyboard** | Captures typed text |
   | **Mouse** | Detects movements and clicks and turns them into cursor movement |
   | **Touchscreen** | Combines input and output by detecting touches right on the display |
   | **Scanner** | Turns paper documents into digital data |
   | **Microphone** | Captures sound |

4. **Input data**: The actual information being sent in. It can be:
   - **Text** (from a keyboard)
   - **Audio** (from a microphone)
   - **Images or video** (from a camera)
   - **Sensor signals** (such as temperature, light, or motion readings from a **sensor**, a device that measures something in the real world)

   Input data can also include commands, raw numbers, or touch gestures. The type and quality of the input data affect how the computer handles it.

### Worked Example

**Task:** You press the letter `A` on a keyboard.

| Step | Element | What happens |
|------|---------|--------------|
| 1 | Input device | The keyboard detects the key press |
| 2 | Input controller | The signal is prepared and passed along |
| 3 | Input interface | The USB port carries the signal to the computer |
| 4 | Input data | The computer receives the data "A" |

### Activity

For each situation, name the input device and the type of input data.

a. You speak into a headset during a video call.
b. You photograph a page of your notes with a phone camera.
c. A chip in a smart home reads the room temperature.

<details>
<summary><b>Answer</b></summary>

a. Input device: **microphone**. Input data: **audio**.
b. Input device: **camera**. Input data: **images**.
c. Input device: **sensor**. Input data: **sensor signals** (temperature).

</details>

---

## 1.2.2 Data Processing

### Explanation

**Processing** means working on the input data by following the program's instructions. The **central processing unit (CPU)** does most of this work. Once the input interface delivers the data, the CPU:

- **Analyzes** the data and converts it into a form the computer can use.
- **Executes** (carries out) the needed operations. For example, if you press a key, the CPU recognizes it, converts it to binary, and triggers the matching action, like showing a letter on the screen.
- **Communicates** with memory, storage, and output devices to finish bigger tasks.

A computer is **programmable**, which means it can run different sets of instructions. This is what makes it useful for so many different jobs.

**Data representation**

Computers store data using the **binary system**. A **bit** (short for *binary digit*) is a single `0` or `1`. You can think of a bit like a light bulb: it is either **off (0)** or **on (1)**. In logic, `1` can also mean **True** and `0` can mean **False**.

[insert image about a light bulb off (0) and a light bulb on (1)]

One bit is too small to hold anything useful, so computers **string many bits together** into a line of 1s and 0s.

**ASCII**

To turn text into binary, computers use a code. **ASCII** (American Standard Code for Information Interchange) is a **character encoding** scheme, which means a system that gives every letter, digit, and symbol its own number. ASCII uses **7 bits** for each character, which gives 128 different combinations (from `0000000` to `1111111`, or 0 to 127 in decimal). Thanks to ASCII, the CPU can turn binary into text that people can read.

| Character | ASCII code | Binary code |
|-----------|-----------|-------------|
| null character | 0 | 0000000 |
| a | 97 | 1100001 |
| b | 98 | 1100010 |
| c | 99 | 1100011 |
| A | 65 | 1000001 |
| B | 66 | 1000010 |
| C | 67 | 1000011 |
| % | 37 | 0100101 |
| + | 43 | 0101011 |
| 0 | 48 | 0110000 |
| 1 | 49 | 0110001 |
| Delete | 127 | 1111111 |

### Worked Example

**Task:** How does the computer store the word `Cab`?

Look up each letter in the ASCII table:

| Letter | ASCII code | Binary code |
|--------|-----------|-------------|
| C | 67 | 1000011 |
| a | 97 | 1100001 |
| b | 98 | 1100010 |

So `Cab` is stored as: `1000011 1100001 1100010`

### Activity

Use the ASCII table above to answer:

a. What is the binary code for `B`?
b. What is the binary code for `+`?
c. Which character does `0110001` stand for?
d. How many different characters can 7-bit ASCII represent?

<details>
<summary><b>Answer</b></summary>

a. `1000010`
b. `0101011`
c. `1` (the digit one, ASCII 49)
d. **128** characters (2 to the power of 7)

</details>

---

## 1.2.3 Storage

### Explanation

After data is processed, the computer often needs to **keep** it. **Storage** is the part of the computer that saves data so it can be used later. There are two main kinds:

- **Memory (main memory)**: Fast, temporary space the computer uses while it is working. It is usually **volatile**, which means its contents are lost when the power is turned off. The most common type is **RAM** (Random Access Memory).
- **Secondary storage**: Slower but permanent space that keeps data even when the power is off (this is called **non-volatile**). Examples include a **hard disk drive (HDD)**, which stores data on spinning magnetic disks, and a **solid-state drive (SSD)**, which stores data on fast electronic chips with no moving parts.

| Feature | Memory (RAM) | Secondary storage (HDD / SSD) |
|---------|--------------|-------------------------------|
| Speed | Very fast | Slower |
| Keeps data when powered off? | No | Yes |
| Typical size | Smaller | Larger |
| Used for | Programs and data currently in use | Files you want to keep |

[insert image about the difference between RAM and a hard drive / SSD]

### Worked Example

**Task:** You write an essay in a word processor.

1. While you type, the essay is held in **RAM** so the computer can change it quickly.
2. When you click **Save**, the essay is copied to the **SSD**.
3. When you shut down the computer, RAM is cleared, but the saved essay stays safe on the SSD.

### Activity

Decide whether each item is memory (RAM) or secondary storage:

a. Holds a game while you are playing it
b. Keeps your photos after you turn off the computer
c. Loses its contents when the power is off

<details>
<summary><b>Answer</b></summary>

a. **Memory (RAM)**
b. **Secondary storage**
c. **Memory (RAM)**

</details>

---

## 1.2.4 Output

### Explanation

**Output** is the result the computer sends back to the user after processing. **Output devices** are the hardware that presents this result:

| Device | What it does |
|--------|--------------|
| **Monitor** | Displays text, images, and video on a screen |
| **Printer** | Puts text or images on paper |
| **Speakers** | Play sound |
| **Touchscreen** | Shows output and also accepts input |

Output devices connect to the computer through ports, in the same way input devices do. Some devices, like a touchscreen, work as both input *and* output.

[insert image about common output devices: monitor, printer, and speakers]

### Worked Example

**Task:** You press **Print** on a finished report.

| Step | What happens |
|------|--------------|
| 1 | The CPU sends the report data toward the printer |
| 2 | The data travels through a port (for example, USB) to the printer |
| 3 | The printer turns the data into a page of paper |

### Activity

Name the best output device for each result:

a. You want to hear a song.
b. You want a paper copy of a form.
c. You want to watch a video.

<details>
<summary><b>Answer</b></summary>

a. **Speakers**
b. **Printer**
c. **Monitor**

</details>

---

# 1.3 Different Types of Computers

## Explanation

Computers come in many sizes. They all follow the same basic workflow (input, processing, storage, output), but they are built for different jobs.

| Type | What it is | Examples |
|------|------------|----------|
| **Personal computer (PC)** | A computer made for one person at a time | Desktop, laptop |
| **Smartphone / tablet** | A small, portable computer you control by touch | Phone, tablet |
| **Server** | A computer that shares data or services with many other computers over a network | Website server, file server |
| **Supercomputer** | An extremely powerful computer for very large calculations | Weather forecasting, scientific research |
| **Embedded computer** | A tiny computer built inside another device to control it | Washing machine, car, smart TV |

A **network** is a group of computers that are connected so they can share data.

[insert image about different types of computers: desktop, laptop, smartphone, server, supercomputer, embedded device]

## Worked Example

**Task:** Which type of computer fits each situation?

| Situation | Type of computer | Why |
|-----------|------------------|-----|
| A student writes a report at home | Personal computer | Made for one person's everyday use |
| A video site sends movies to millions of viewers | Server | Shares data with many users over a network |
| Scientists simulate a storm that may hit next week | Supercomputer | Needs huge calculating power |
| A microwave controls its heating time | Embedded computer | A tiny computer built inside the appliance |

## Activity

Name the type of computer in each situation:

a. A phone used to check the weather.
b. The small computer inside a car that controls the engine.
c. A powerful machine used to model how a new medicine works.
d. A computer that stores and shares your school's files with all students.

<details>
<summary><b>Answer</b></summary>

a. **Smartphone**
b. **Embedded computer**
c. **Supercomputer**
d. **Server**

</details>

---

## Stage 1 Summary

- A **computer** takes **data** (input), processes it using a **program**, and gives a result (output). It can also save data (storage).
- The **Turing model** shows that a computer's output depends on its input data and its program.
- The **von Neumann model** splits a computer into **Memory**, **ALU**, **Control Unit**, and **Input/Output**, and stores programs and data together.
- Computers have **hardware** (physical parts), **software** (programs), and **data**.
- Computers use **binary** (0s and 1s). **ASCII** turns characters into binary codes.
- The basic workflow is **Input → Processing → Storage → Output**.
- Computers come in many types, such as PCs, smartphones, servers, supercomputers, and embedded computers.