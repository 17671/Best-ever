# Stage 1: Computers and Data

## Learning Goals

By the end of this stage, you will be able to:

<<<<<<< HEAD
1. Identify the core physical components of a computer and explain their basic functions.
=======
1. Identify the core physical components of computers and explain their basic functions.
>>>>>>> origin/topic-1.1

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
<<<<<<< HEAD
| 1 | **Input** | Receives data from the outside world | Typing on a keyboard, moving a mouse |
=======
| 1 | **Input** | Receives data from the outside world | Typing on a keyboard, moving a mouse, a sensor reading |
>>>>>>> origin/topic-1.1
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
<<<<<<< HEAD
- A set of **rules** that tell the head what to do next, based on the symbol it sees.
=======
- A set of **rules** that tell the head what to do next, based on the symbol it sees and its current state.
>>>>>>> origin/topic-1.1

[insert image about a Turing Machine with its tape and head]

From this idea comes the **Turing model**, which describes a computer as a **programmable data processor**. *Programmable* means you can change what the computer does by changing its program. The computer is treated like a **black box**: a device where you only see what goes in and what comes out, not what happens inside.

[insert image about a black box diagram: Input data -> Computer -> Output data]

<<<<<<< HEAD
In this model, the output depends on **two things**: the **input data** and the **program**. Changing either one can change the result. But running the *same program* with the *same input* always gives the *same output*.

> **Note:** This model is a little too broad. Even a simple calculator fits this description, but we don't usually call a calculator a full computer.

Turing's work also showed that any problem that *can* be solved by following steps can be solved by a computer, as long as it has the correct program.

=======
In this model, the output depends on **two things**: the **input data** and the **program**. Changing either one can change the result. But running the *same program* with the *same input* always gives the *same output*. Turing's work also showed that any problem that *can* be solved by following steps can be solved by a computer, as long as it has the correct program.

> **Note:** This model is a little too broad. Even a simple calculator fits this description, but we don't usually call a calculator a full computer.

>>>>>>> origin/topic-1.1
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

<<<<<<< HEAD
**Memory** is the part of the computer that holds programs and data while the computer is working. Before this idea, early computers had to be rewired by hand every time they needed to do a new job. With the von Neumann model, switching tasks is as easy as loading a different program.
=======
**Memory** is the part of the computer that holds programs and data while the computer is working. Before this idea, early computers had to be rewired by hand every time they needed to do a new job. With the von Neumann model, switching tasks is as easy as loading a different program. This model is the base of most modern computers.
>>>>>>> origin/topic-1.1

The **von Neumann model** splits a computer into four parts, called **subsystems**:

| Subsystem | What it does |
|-----------|--------------|
| **Memory** | Stores both programs and data |
| **Arithmetic Logic Unit (ALU)** | Does the math (like adding) and the logic (like comparing two numbers) |
| **Control Unit** | Manages and directs all the other parts, like a traffic controller |
| **Input/Output** | Moves data between the computer and the outside world |

<<<<<<< HEAD
The control unit repeats a simple cycle: it **fetches** (gets) an instruction from memory, then **executes** (carries out) it, then moves on to the next one. This keeps programs running in an orderly and predictable way.
=======
The control unit repeats a simple cycle: it **fetches** (gets) an instruction from memory, then **executes** (carries out) it, then moves on to the next one, one after another. This keeps programs running in an orderly and predictable way.
>>>>>>> origin/topic-1.1

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

<<<<<<< HEAD
[insert image about input example (keyboard to computer) and output example (computer to printer)]

Computers store and process data in **binary**, a number system that uses only two digits: `0` and `1`. Numbers, text, pictures, and sound must all be converted into binary before a computer can work with them. **Software** is what lets the hardware and the data work together, because it tells the hardware how to handle the data.
=======
[insert image about an input example (keyboard to screen) and an output example (screen to printer)]

Computers store and process data in **binary**, a number system that uses only two digits: `0` and `1`. Numbers, text, pictures, and sound must all be converted into binary before a computer can work with them. **Software** is what lets the hardware and the data work together, because it tells the hardware how to handle the data. The idea of software began with early computers, where programs were set up by hand.
>>>>>>> origin/topic-1.1

Software has four key parts:

1. **Stored programs**: Modern computers keep both programs and data in memory. Early computers needed to be set up by hand for each task.

   [insert image about memory split into a Program section and a Data section]

2. **Sequence of instructions**: A program is a series of instructions that work on data. The same instructions can be reused and rearranged to build different programs.

   [insert image about a four-step instruction list: input first number, input second number, add and store, output result]

3. **Algorithms**: An **algorithm** is a step-by-step set of rules for solving a problem. Programmers plan an algorithm *before* they write a program.

   [insert image about an algorithm flowchart: Input -> Set of rules -> Output]

<<<<<<< HEAD
4. **Languages**: Early computers only understood **machine language**, which is written entirely in binary. Later, **symbolic languages** were created, which use letters and symbols so people can write programs more easily. One early standard is **ASCII** (explained in section 1.2.2).
=======
4. **Languages**: Early computers only understood **machine language**, which is written entirely in binary. Later, **symbolic languages** were created, which use letters and symbols so people can write programs more easily. The first standard one is **ASCII** (explained in section 1.2.2), which gives every character its own number and binary code:

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
>>>>>>> origin/topic-1.1

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

<<<<<<< HEAD
A **workflow** is the path that data follows from start to finish. In a computer, data moves through four stages:

**Input → Processing → Storage → Output**

[insert image about the computer workflow: input, processing, storage, output]
=======
A **workflow** is the path that data follows from start to finish. In a computer, data moves through four parts:

**Input → Processing → Output**, with **Storage** connected to the processing step so data can be saved and retrieved.

[insert image about the computer workflow: input, processing, output, with storage connected to processing]
>>>>>>> origin/topic-1.1

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

<<<<<<< HEAD
**Processing** means working on the input data by following the program's instructions. The **central processing unit (CPU)** does most of this work. Once the input interface delivers the data, the CPU:
=======
**Processing** means working on the input data by following the program's instructions, usually using logic and arithmetic. The **central processing unit (CPU)** does most of this work. It is the **processing unit** of the computer. Once the input interface delivers the data, the CPU:
>>>>>>> origin/topic-1.1

- **Analyzes** the data and converts it into a form the computer can use.
- **Executes** (carries out) the needed operations. For example, if you press a key, the CPU recognizes it, converts it to binary, and triggers the matching action, like showing a letter on the screen.
- **Communicates** with memory, storage, and output devices to finish bigger tasks.

A computer is **programmable**, which means it can run different sets of instructions. This is what makes it useful for so many different jobs.

**Data representation**

Computers store data using the **binary system**. A **bit** (short for *binary digit*) is a single `0` or `1`. You can think of a bit like a light bulb: it is either **off (0)** or **on (1)**. In logic, `1` can also mean **True** and `0` can mean **False**.

[insert image about a light bulb off (0) and a light bulb on (1)]

<<<<<<< HEAD
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
=======
One bit is too small to hold anything useful, so computers **string many bits together** into a line of 1s and 0s. Binary makes it easy for the hardware to store and work with information. From binary, computers can build bigger kinds of data, such as **integers** (whole numbers), **floating-point numbers** (numbers with a decimal point), and **characters** (letters and symbols).

**Reading binary**

Each bit has a **place value**, which is a **power of 2**. A power of 2 means 2 multiplied by itself a number of times (for example, 2³ = 2 × 2 × 2 = 8). Place values count **from right to left**, starting at 2⁰:

| Power | 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|-------|----|----|----|----|----|----|----|----|
| Value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

To turn a binary number into a **decimal** number (the normal numbers we use every day), keep the values where the bit is **1** and add them up.

[insert image about binary place values 2⁷ to 2⁰ above a string of bits]

**ASCII**

To turn text into binary, computers use a code. **ASCII** (American Standard Code for Information Interchange) is a **character encoding** scheme, which means a system that gives every letter, digit, and symbol its own number. ASCII uses **7 bits** for each character, which gives 128 different combinations (from `0000000` to `1111111`, or 0 to 127 in decimal). The computer can "call" a character's ASCII number to display that character. For example, the letter **A** has the number **65**. Thanks to ASCII, the computer can turn binary into text that people can read.

Characters are usually grouped into a **character set**, which is the collection of characters a system can use. A character set includes:

- **Alphanumeric data**: letters and numbers.
- **Symbols**: such as `?`, `&`, and `:`.
- **Control characters**: special characters that give commands instead of showing a symbol, such as Backspace, Horizontal Tab, and Escape.

### Worked Example

**Task 1:** Convert `00010011` to decimal.

| Bit | 0 | 0 | 0 | 1 | 0 | 0 | 1 | 1 |
|-----|---|---|---|---|---|---|---|---|
| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| Kept? | No | No | No | **Yes** | No | No | **Yes** | **Yes** |

16 + 2 + 1 = **19**

**Task 2:** How does the computer know `1000001` is the letter A?

1. Add the place values of the 1s: 64 + 1 = **65**
2. Look up 65 in the ASCII table: it is the character **A**.

### Activity

a. Convert `00101101` to decimal.
b. What decimal number is `01000001`, and which character does it show?
c. What is the binary code for `B`? (Use the ASCII table in 1.1.3.)
d. Is Escape an alphanumeric character, a symbol, or a control character?
>>>>>>> origin/topic-1.1

<details>
<summary><b>Answer</b></summary>

<<<<<<< HEAD
a. `1000010`
b. `0101011`
c. `1` (the digit one, ASCII 49)
d. **128** characters (2 to the power of 7)
=======
a. 32 + 8 + 4 + 1 = **45**
b. 64 + 1 = **65**, which is the letter **A**
c. `1000010`
d. A **control character**
>>>>>>> origin/topic-1.1

</details>

---

<<<<<<< HEAD
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
=======
## 1.2.3 Output

### Explanation

**Output** is the data or information that a computer sends to an outside device or to the user after it has processed the input. The output system has three parts:

1. **Output interface**: The part that sends processed data from inside the computer to the outside world (to a user or another device). It has **hardware** (the output devices) and **software** (called **drivers**, small programs that let the computer communicate with a device).
2. **Output devices**: Devices that take the processed data and show it in a form people can use:

   | Device | What it does |
   |--------|--------------|
   | **Monitor (display)** | Turns digital data into pictures, text, or video |
   | **Printer** | Makes a **hard copy** (a paper copy) of documents or images |
   | **Speakers** | Play sound after the computer has processed the audio data |

3. **Digital-to-analog conversion**: Computers work with **digital signals** (made of 0s and 1s), but some devices, like speakers, need **analog signals** (smooth, continuously changing waves). A **sound card** in the computer converts digital audio files into analog waves that speakers can play. The part that does this job is a **digital-to-analog converter (DAC)**. Inside a DAC, the digital input is first held in a register, then turned into voltage levels, added together, boosted by an amplifier, and sent out as an analog signal.

[insert image about a digital-to-analog converter turning digital input into an analog output]

**How the process works:** After the CPU finishes processing, it sends the results to the correct output system. The data travels to the connected device, where it is displayed, printed, or played. The format of the output depends on the type of data and the device being used.

[insert image about the Input -> Process -> Output flow with Storage connected to Process]

### Worked Example

**Task:** You play a song on your computer.

| Step | What happens |
|------|--------------|
| 1 | The CPU processes the digital audio file |
| 2 | The CPU sends the data to the output system |
| 3 | The **sound card (DAC)** converts the digital audio to analog waves |
| 4 | The **speakers** play the sound |

### Activity

Name the best output device for each result, and say whether a digital-to-analog conversion is needed:

a. You want a paper copy of a form.
b. You want to watch a photo slideshow.
c. You want to hear a voice message.
>>>>>>> origin/topic-1.1

<details>
<summary><b>Answer</b></summary>

<<<<<<< HEAD
a. **Speakers**
b. **Printer**
c. **Monitor**
=======
a. **Printer.** No conversion is needed.
b. **Monitor.** No conversion is needed.
c. **Speakers.** Yes, a digital-to-analog conversion is needed to turn the digital audio into sound waves.

</details>

---

## 1.2.4 Storage

### Explanation

**Storage** is the part of a computer that **saves and keeps data**. There are two time scales:

- **Primary storage** (short term): Fast memory the computer uses while it is working, such as **RAM** (Random Access Memory). It is usually **volatile**, which means its contents are lost when the power is turned off.
- **Secondary storage** (long term): Storage that keeps data even when the computer is powered off. This is called **non-volatile** storage. Examples are a **hard disk drive (HDD)**, which stores data on spinning magnetic disks, and a **solid-state drive (SSD)**, which stores data on electronic chips with no moving parts.

Storage holds both **programs** and **data**. In the von Neumann model, storage keeps the program's instructions and the data those instructions work on. In modern computers, everything is stored in **binary**, so the same patterns of 0s and 1s can stand for text, images, or videos.

| Feature | Primary storage (RAM) | Secondary storage (HDD / SSD) |
|---------|----------------------|-------------------------------|
| Time scale | Short term | Long term |
| Speed | Very fast | Slower |
| Keeps data when powered off? | No | Yes |
| Used for | Programs and data currently in use | Files you want to keep |

[insert image about primary storage (RAM) and secondary storage (a drive) in a computer]

### Worked Example

**Task:** You edit a photo and save it.

| Step | Where is the photo? |
|------|---------------------|
| 1 | You open the photo: it is loaded into **primary storage (RAM)** so you can edit it quickly |
| 2 | You click Save: it is copied to **secondary storage** (for example, the SSD) |
| 3 | You switch off the computer: RAM is cleared, but the saved photo remains in secondary storage |

### Activity

Is each example primary or secondary storage?

a. The place where a game is held while it is running.
b. A drive that keeps your documents after the computer is turned off.
c. Storage that loses its contents when the power is off.

<details>
<summary><b>Answer</b></summary>

a. **Primary storage** (RAM)
b. **Secondary storage**
c. **Primary storage** (RAM)
>>>>>>> origin/topic-1.1

</details>

---

# 1.3 Different Types of Computers

## Explanation

<<<<<<< HEAD
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
=======
Today, there are many kinds of computers, each made for different needs and jobs. They all follow the same basic workflow (input, processing, output, and storage).

**1. Personal Computers (PCs)**

- **Desktop computers**: Traditional computers with a separate monitor, keyboard, and CPU tower. They stay in one place and usually offer high processing power.
- **Laptop computers**: Portable computers where the screen, keyboard, and CPU are built into one unit. They balance performance with the ability to carry them around.

[insert image about a desktop computer setup]

**2. Mobile Devices**

- **Smartphones**: Pocket-sized devices with powerful computing abilities. They make calls and send messages, browse the Internet, and run many kinds of apps.
- **Tablets**: Larger touchscreen devices that sit between a smartphone and a PC. They are great for casual browsing, watching media, and light work.

[insert image about a smartphone and a tablet]

**3. Servers and Supercomputers**

- **Servers**: Specialized computers that manage resources and provide services to other devices on a **network** (a group of connected computers that share data). They are used for **web hosting** (keeping websites online), **database management** (storing and organizing large amounts of data), and network communication.
- **Supercomputers**: Extremely fast systems built for very complex calculations and huge amounts of data. They are used for scientific simulations, climate modeling, and advanced data analysis.

[insert image about a server room and a supercomputer]

**4. Embedded Systems**

**Embedded systems** are small, specialized computers built into everyday objects, such as appliances, cars, factory machines, and medical equipment. Each one performs a specific job and is important for automation, control, and monitoring.

[insert image about an embedded system, such as a car engine management module]

| Type | Main purpose | Examples |
|------|--------------|----------|
| Desktop | Powerful, stationary use | Office computer |
| Laptop | Portable everyday computing | School or work laptop |
| Smartphone | Calls, messaging, apps in your pocket | Phone |
| Tablet | Browsing and media on a touchscreen | Tablet |
| Server | Provides services to other devices | Web server |
| Supercomputer | Huge, complex calculations | Climate model |
| Embedded system | One built-in job inside a device | Car engine controller, washing machine |

## Worked Example

**Task:** Pick the best type of computer for each person.

| Person's need | Best type | Why |
|---------------|-----------|-----|
| A video editor needs strong power at a fixed desk | Desktop | High processing power for stationary use |
| A student takes notes in different classrooms | Laptop | Portable, with a built-in screen and keyboard |
| A company runs a website for thousands of visitors | Server | Provides services to many devices on a network |
| A scientist models the climate | Supercomputer | Handles very complex calculations at high speed |
>>>>>>> origin/topic-1.1

## Activity

Name the type of computer in each situation:

<<<<<<< HEAD
a. A phone used to check the weather.
b. The small computer inside a car that controls the engine.
c. A powerful machine used to model how a new medicine works.
d. A computer that stores and shares your school's files with all students.
=======
a. The small computer that controls the temperature inside a smart oven.
b. A touchscreen device used for reading and watching videos on the couch.
c. A computer that stores and shares your school's files with every student.
d. A system used to simulate how a storm will move across the ocean.
>>>>>>> origin/topic-1.1

<details>
<summary><b>Answer</b></summary>

<<<<<<< HEAD
a. **Smartphone**
b. **Embedded computer**
c. **Supercomputer**
d. **Server**
=======
a. **Embedded system**
b. **Tablet**
c. **Server**
d. **Supercomputer**
>>>>>>> origin/topic-1.1

</details>

---

## Stage 1 Summary

- A **computer** takes **data** (input), processes it using a **program**, and gives a result (output). It can also save data (storage).
- The **Turing model** shows that a computer's output depends on its input data and its program.
- The **von Neumann model** splits a computer into **Memory**, **ALU**, **Control Unit**, and **Input/Output**, and stores programs and data together.
- Computers have **hardware** (physical parts), **software** (programs), and **data**.
<<<<<<< HEAD
- Computers use **binary** (0s and 1s). **ASCII** turns characters into binary codes.
- The basic workflow is **Input → Processing → Storage → Output**.
- Computers come in many types, such as PCs, smartphones, servers, supercomputers, and embedded computers.
=======
- Computers use **binary** (0s and 1s). Each bit has a place value, and **ASCII** turns characters into binary codes.
- The basic workflow is **Input → Processing → Output**, with **Storage** saving data along the way.
- Output devices such as monitors, printers, and speakers present results, and speakers need **digital-to-analog conversion**.
- **Primary storage** (RAM) is fast and short term. **Secondary storage** (HDD/SSD) keeps data long term.
- Computers come in many types: **PCs, mobile devices, servers, supercomputers, and embedded systems**.

---

# Stage 2: Number Systems

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions. *(Computers use binary because their hardware has two states, on and off. Number systems are how we read and write that data.)*
2. Explain what a number system is and describe the binary, decimal, and hexadecimal systems.
3. Convert between binary and decimal.
4. Convert between hexadecimal and binary.
5. Convert between hexadecimal and decimal.

**Topics covered:**

- Number System Overview
- Binary Number System
- Decimal to Binary and Binary to Decimal
- Hexadecimal to Binary and Binary to Hexadecimal
- Hexadecimal to Decimal and Decimal to Hexadecimal

---

# 2.1 Number System Overview

## Explanation

A **number system** is a way of writing numbers using a set of symbols, called **digits**. Every number system has a **base**. The base tells you **how many different digits** the system uses before it "rolls over" to the next place. (In everyday counting, we roll over after 9: we write 10, which means "one group of ten and zero ones".)

The most common number systems in computing are:

| System | Base | Digits used | Example |
|--------|------|-------------|---------|
| **Binary** | 2 | 0, 1 | `1101` |
| **Octal** | 8 | 0 to 7 | `157` |
| **Decimal** | 10 | 0 to 9 | `106` |
| **Hexadecimal** | 16 | 0 to 9 and A to F | `6A` |

All of these are **positional number systems**. That means the **position** of a digit decides its value. Each position has a **place value**, which is a **power of the base**. A **power** means the base multiplied by itself a number of times (for example, 2³ = 2 × 2 × 2 = 8, and any base to the power of 0 equals 1).

When two systems are mixed in the same text, a small number written after the value shows the base. For example, `157₈` is in octal and `157₁₀` is in decimal.

The **octal** system (base 8) is less common, but it is a short way to write binary, because 8 is a power of 2.

[insert image about number systems: binary, octal, decimal, and hexadecimal side by side]

## Worked Example

**Task:** Find the value of the decimal number `352`, and the octal number `157₈`.

**Decimal `352`** (base 10):

| Digit | 3 | 5 | 2 |
|-------|---|---|---|
| Place value | 10² = 100 | 10¹ = 10 | 10⁰ = 1 |
| Digit × place value | 300 | 50 | 2 |

300 + 50 + 2 = **352**

**Octal `157₈`** (base 8):

| Digit | 1 | 5 | 7 |
|-------|---|---|---|
| Place value | 8² = 64 | 8¹ = 8 | 8⁰ = 1 |
| Digit × place value | 64 | 40 | 7 |

64 + 40 + 7 = **111** in decimal, so `157₈ = 111₁₀`

## Activity

a. What is the base of the binary system, and which digits does it use?
b. How many different digits does the hexadecimal system use?
c. Find the decimal value of the octal number `24₈`.

<details>
<summary><b>Answer</b></summary>

a. Base **2**. It uses the digits **0 and 1**.
b. **16** digits (0 to 9 and A to F).
c. (2 × 8) + (4 × 1) = 16 + 4 = **20**

</details>

---

# 2.2 Binary Number System

## Explanation

The **binary number system** (base 2) uses only two digits: `0` and `1`. A single binary digit is called a **bit**. Binary fits computers well, because the hardware inside only has two states: **off (0)** and **on (1)**, like a light bulb.

Each place in a binary number is a **power of 2**. Place values count **from right to left**, starting at 2⁰:

| Power | 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|-------|----|----|----|----|----|----|----|----|
| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

Two useful terms:

- **Most Significant Bit (MSB)**: The leftmost bit. It has the biggest place value.
- **Least Significant Bit (LSB)**: The rightmost bit. It has the smallest place value.

In logic, a `1` can also mean **True** and a `0` can mean **False**.

[insert image about binary place values 2⁷ to 2⁰ above a string of bits, with MSB and LSB labeled]

## Worked Example

**Task:** Write out the place value of each bit in `00010011`, and say which bits are True.

| Bit | 0 | 0 | 0 | 1 | 0 | 0 | 1 | 1 |
|-----|---|---|---|---|---|---|---|---|
| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| True / False | False | False | False | **True** | False | False | **True** | **True** |

- The **MSB** is the leftmost `0` (place value 128).
- The **LSB** is the rightmost `1` (place value 1).

## Activity

Look at the binary number `10100110`.

a. What is the MSB, and what is its place value?
b. What is the LSB, and what is its place value?
c. Which place values are True (bit = 1)?

<details>
<summary><b>Answer</b></summary>

a. The MSB is `1`, with place value **128**.
b. The LSB is `0`, with place value **1**.
c. The bits that are 1 are at place values **128, 32, 4, and 2**.

</details>

---

# 2.3 Decimal to Binary and Binary to Decimal

## Binary to Decimal

### Explanation

To turn a binary number into a **decimal** number:

1. Write the place value above each bit.
2. Keep the place values where the bit is **1** (True). Ignore the ones where the bit is **0** (False).
3. **Add** the kept values.

### Worked Example

**Task 1:** Convert `00010011` to decimal.

| Bit | 0 | 0 | 0 | 1 | 0 | 0 | 1 | 1 |
|-----|---|---|---|---|---|---|---|---|
| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| Kept? | No | No | No | **Yes** | No | No | **Yes** | **Yes** |

16 + 2 + 1 = **19**

**Task 2:** Convert `1101010` to decimal.

1 × 2⁶ + 1 × 2⁵ + 0 × 2⁴ + 1 × 2³ + 0 × 2² + 1 × 2¹ + 0 × 2⁰
= 64 + 32 + 0 + 8 + 0 + 2 + 0
= **106**

### Activity

Convert to decimal:

a. `11001`
b. `1011011`

<details>
<summary><b>Answer</b></summary>

a. 16 + 8 + 0 + 0 + 1 = **25**
b. 64 + 0 + 16 + 8 + 0 + 2 + 1 = **91**

</details>

---

## Decimal to Binary

### Explanation

To turn a decimal number into binary, use **repeated division by 2**:

1. Divide the number by 2. Write down the **remainder** (what is left over, either 0 or 1).
2. Divide the result (the **quotient**) by 2 again, and write the new remainder.
3. Keep going until the quotient is **0**.
4. Read the remainders **from the last to the first** (bottom to top). That is the binary number.

[insert image about repeated division by 2 with remainders read from bottom to top]

### Worked Example

**Task:** Convert `19` to binary.

| Division | Quotient | Remainder |
|----------|----------|-----------|
| 19 ÷ 2 | 9 | **1** |
| 9 ÷ 2 | 4 | **1** |
| 4 ÷ 2 | 2 | **0** |
| 2 ÷ 2 | 1 | **0** |
| 1 ÷ 2 | 0 | **1** |

Read the remainders from bottom to top: `10011`

Add zeros on the left to fill 8 bits (this does not change the value): `00010011`

**Check:** 16 + 2 + 1 = 19 ✓

### Activity

Convert to binary:

a. `45`
b. `100`

<details>
<summary><b>Answer</b></summary>

a. 45 ÷ 2 = 22 r **1**, 22 ÷ 2 = 11 r **0**, 11 ÷ 2 = 5 r **1**, 5 ÷ 2 = 2 r **1**, 2 ÷ 2 = 1 r **0**, 1 ÷ 2 = 0 r **1**. Reading from the bottom: **101101** (check: 32 + 8 + 4 + 1 = 45).
b. 100 ÷ 2 = 50 r **0**, 50 ÷ 2 = 25 r **0**, 25 ÷ 2 = 12 r **1**, 12 ÷ 2 = 6 r **0**, 6 ÷ 2 = 3 r **0**, 3 ÷ 2 = 1 r **1**, 1 ÷ 2 = 0 r **1**. Reading from the bottom: **1100100** (check: 64 + 32 + 4 = 100).

</details>

---

# 2.4 Hexadecimal to Binary and Binary to Hexadecimal

## Explanation

The **hexadecimal system**, or **hex** (base 16), uses sixteen digits: `0` to `9`, then letters for the larger values:

| Hex digit | A | B | C | D | E | F |
|-----------|---|---|---|---|---|---|
| Decimal value | 10 | 11 | 12 | 13 | 14 | 15 |

Hex is very popular in computing because:

- **It is compact**: A long binary number becomes much shorter. For example, a 16-bit binary number can be written with just 4 hex digits.
- **It is easy to read**: People can read and write hex more easily than long strings of 1s and 0s.
- **It is common in programming**: Memory addresses, color codes in web design (like `#FF0000` for red), and machine code instructions are often written in hex.

There are two ways to convert between binary and hex:

- **Indirect method**: First convert to another system (such as decimal), then convert to the final system.
- **Direct method (grouping)**: Because there are 16 hex digits, each hex digit can be written with exactly **4 bits**. So you can split the binary number into groups of 4 bits and swap each group for a hex digit.

**Hex and binary table:**

| Hex | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
|-----|---|---|---|---|---|---|---|---|
| Binary | 0000 | 0001 | 0010 | 0011 | 0100 | 0101 | 0110 | 0111 |

| Hex | 8 | 9 | A | B | C | D | E | F |
|-----|---|---|---|---|---|---|---|---|
| Binary | 1000 | 1001 | 1010 | 1011 | 1100 | 1101 | 1110 | 1111 |

**Binary to hex (grouping):**

1. Start at the **right** end and split the bits into groups of 4.
2. If the leftmost group has fewer than 4 bits, add **zeros on the left** to complete it. This does not change the value, just like 007 is the same as 7.
3. Replace each group with its hex digit from the table.

**Hex to binary:** Replace each hex digit with its 4-bit group from the table.

[insert image about grouping a binary number into 4-bit groups and replacing each group with a hex digit]

## Worked Example

**Task 1 (indirect method):** Convert `1101010` to hex.

1. Convert to decimal: 64 + 32 + 0 + 8 + 0 + 2 + 0 = **106**
2. Convert 106 to hex: 106 = (6 × 16) + 10, and 10 is written as A. So the answer is **6A₁₆**.

**Task 2 (grouping method):** Convert `1010101101001` to hex.

1. Split into groups of 4 from the right: `1 | 0101 | 0110 | 1001`
2. Add three zeros on the left to fill the first group: `0001 | 0101 | 0110 | 1001`
3. Replace each group: 0001 = **1**, 0101 = **5**, 0110 = **6**, 1001 = **9**

Answer: **1569₁₆**

**Task 3 (hex to binary):** Convert `3F2₁₆` to binary.

3 = `0011`, F = `1111`, 2 = `0010`

Answer: **001111110010** (the leading zeros can be dropped: `1111110010`)

## Activity

a. Use grouping to convert `10111100` to hex.
b. Use grouping to convert `101111` to hex. (Remember to fill the first group with zeros.)
c. Convert `A5₁₆` to binary.

<details>
<summary><b>Answer</b></summary>

a. `1011 | 1100` → B and C → **BC**
b. Add zeros: `0010 | 1111` → 2 and F → **2F**
c. A = `1010`, 5 = `0101` → **10100101**

</details>

---

# 2.5 Hexadecimal to Decimal and Decimal to Hexadecimal

## Hexadecimal to Decimal

### Explanation

Hex numbers use **powers of 16** as place values. Positions are counted from right to left, starting at 16⁰:

| Power | 16³ | 16² | 16¹ | 16⁰ |
|-------|-----|-----|-----|-----|
| Place value | 4096 | 256 | 16 | 1 |

Hex can also have a **fractional part** (the part after the hex point, like the decimal point). Those places count from left to right as 16⁻¹ = 1/16, 16⁻² = 1/256, 16⁻³ = 1/4096, and so on.

To convert hex to decimal:

1. Change each hex letter to its decimal value (A = 10, B = 11, and so on).
2. Multiply each digit by its place value.
3. Add the results.

[insert image about hexadecimal place values 16³, 16², 16¹, 16⁰ and the fractional places]

### Worked Example

**Task:** Convert `3F2₁₆` to decimal. (F = 15)

| Digit | 3 | F | 2 |
|-------|---|---|---|
| Place value | 16² = 256 | 16¹ = 16 | 16⁰ = 1 |
| Digit × place value | 3 × 256 = 768 | 15 × 16 = 240 | 2 × 1 = 2 |

768 + 240 + 2 = **1010**

### Activity

Convert to decimal:

a. `2F₁₆`
b. `A5₁₆`
c. `1C₁₆`

<details>
<summary><b>Answer</b></summary>

a. (2 × 16) + (15 × 1) = 32 + 15 = **47**
b. (10 × 16) + (5 × 1) = 160 + 5 = **165**
c. (1 × 16) + (12 × 1) = 16 + 12 = **28**

</details>

---

## Decimal to Hexadecimal

### Explanation

To convert a decimal number to hex, use **repeated division by 16**:

1. Divide the number by 16 and write down the **remainder**. If the remainder is 10 to 15, write it as A to F.
2. Divide the quotient by 16 again, and write the new remainder.
3. Keep going until the quotient is **0**.
4. Read the remainders **from last to first** (bottom to top).

### Worked Example

**Task 1:** Convert `106` to hex.

| Division | Quotient | Remainder |
|----------|----------|-----------|
| 106 ÷ 16 | 6 | 10 → **A** |
| 6 ÷ 16 | 0 | **6** |

Read from bottom to top: **6A₁₆** (this matches the answer from section 2.4).

**Task 2:** Convert `1010` to hex.

| Division | Quotient | Remainder |
|----------|----------|-----------|
| 1010 ÷ 16 | 63 | **2** |
| 63 ÷ 16 | 3 | 15 → **F** |
| 3 ÷ 16 | 0 | **3** |

Read from bottom to top: **3F2₁₆**

### Activity

Convert to hex:

a. `255`
b. `300`

<details>
<summary><b>Answer</b></summary>

a. 255 ÷ 16 = 15 r 15 (F), 15 ÷ 16 = 0 r 15 (F). Reading from the bottom: **FF**
b. 300 ÷ 16 = 18 r 12 (C), 18 ÷ 16 = 1 r 2, 1 ÷ 16 = 0 r 1. Reading from the bottom: **12C** (check: 256 + 32 + 12 = 300)

</details>

---

## Stage 2 Summary

- A **number system** writes numbers using digits. Its **base** tells how many digits it uses before rolling over.
- **Binary** (base 2) uses 0 and 1, **octal** (base 8) uses 0 to 7, **decimal** (base 10) uses 0 to 9, and **hexadecimal** (base 16) uses 0 to 9 and A to F.
- In a **positional** number system, each place has a value that is a **power of the base**.
- **Binary to decimal**: Add the place values of the 1s.
- **Decimal to binary**: Divide by 2 again and again, then read the remainders from bottom to top.
- **Binary to hex**: Group the bits in fours (adding zeros on the left if needed) and replace each group with a hex digit. **Hex to binary**: Replace each hex digit with its 4 bits.
- **Hex to decimal**: Multiply each digit by its power of 16 and add. **Decimal to hex**: Divide by 16 again and again, then read the remainders from bottom to top.

---

# Stage 3: Data Storage

## Learning Goals

By the end of this stage you should be able to:

1. Identify the core physical components of a computer that store data and explain their basic functions.
2. Explain how data is stored and retrieved inside a computer.
3. Describe how numbers, text, images, audio and video are represented in binary.
4. Compare primary and secondary storage.
5. Compare common storage devices (HDD, SSD, optical discs, USB drives) and choose the right one for a job.


**Topics covered:**

1. [Definition](#1-definition)
2. [How Does Data Storage Work?](#2-how-does-data-storage-work)
3. [Representing Data in Binary](#3-representing-data-in-binary)
4. [Types of Data Storage](#4-types-of-data-storage-primary-and-secondary)
5. [Data Storage Devices](#5-data-storage-devices-hdd-ssd-usb-drives)
6. [Summary and Revision Checklist](#6-summary-and-revision-checklist)

---

## 1. Definition

### Explanation

**Data** is any information a computer can work with, such as a number, a word, a photo or a song.

**Storage** is the part of a computer that holds data so the **CPU** (Central Processing Unit, the "brain" that carries out instructions) and other components can reach it when they need it.

Storage is not one single part. A computer uses **several kinds** of storage together:

- Some storage is **very fast** but small and temporary.
- Some storage is **slower** but large and permanent.

Two words you will see often:

| Term | Meaning |
|---|---|
| **Volatile** | Loses its data when the power is turned off. |
| **Non-volatile** | Keeps its data even when the power is off. |

### Worked Example

You are writing an essay.

- While you type, the text sits in a fast, temporary storage area. If the power suddenly cuts out, the unsaved text is gone. This storage is **volatile**.
- When you press **Save**, the essay is copied to a permanent storage area. You can switch the computer off and open the essay tomorrow. This storage is **non-volatile**.

### Activity

Write **V** (volatile) or **N** (non-volatile) for each situation:

1. A web page you have open but have not saved.
2. A photo saved on a USB flash drive.
3. A game installed on your computer's drive.
4. The numbers a calculator program is using right now.

### Answer

1. **V**, open and unsaved data lives in temporary storage.
2. **N**, a USB drive keeps data without power.
3. **N**, installed programs are kept permanently.
4. **V**, data in use right now is held in temporary storage.

---

## 2. How Does Data Storage Work?

### Explanation

A computer moves data between storage areas all the time. A simplified journey looks like this:

1. **Secondary storage** (permanent) holds your files and programs.
2. When you open something, the data is copied into **RAM** (fast, temporary memory).
3. The CPU reads from RAM, because it is much quicker than reading from permanent storage.
4. When you save, the data is copied back to secondary storage.

**RAM** acts as a **high-speed buffer** (a waiting area) between the CPU and slower storage devices such as hard drives. It lets the computer quickly find and process the data needed to run applications and carry out commands.

Where does the data travel? Through the **motherboard**, the main circuit board that connects all the parts. Two things on the motherboard affect how smoothly memory and CPU "talk" to each other:

- The **chipset**, a group of chips that manages communication between components.
- The **bus speed**, how fast data can travel along the connecting pathways (the **bus**).

The motherboard also has **memory slots** where RAM modules are plugged in.

### Worked Example

You double-click a video game.

| Step | What happens |
|---|---|
| 1 | The game's files are found on the SSD or hard drive (secondary storage). |
| 2 | The parts of the game that are needed are copied into RAM. |
| 3 | The CPU reads the game's instructions from RAM and runs them. |
| 4 | When you save your progress, a save file is written back to the drive. |

### Activity

Put these steps in the correct order:

- A. The CPU processes the data in RAM.
- B. The file is saved back to the drive.
- C. You open a file stored on the drive.
- D. The file's data is copied into RAM.

### Answer

**C → D → A → B**

You open the file (C), it is copied to RAM (D), the CPU works on it (A), then it is saved back (B).

---

## 3. Representing Data in Binary

### Explanation

Computers are built from electronic switches that are either **on** or **off**. This is why they use **binary**, a number system with only two digits: **0** and **1**.

- A **bit** (binary digit) is a single 0 or 1.
- A **byte** is a group of **8 bits**.

Everything stored in a computer (numbers, text, images, audio, video) is turned into long strings of bits.

**Storage units** (we use 1000 for simplicity; some systems use 1024):

| Unit | Size |
|---|---|
| 1 byte (B) | 8 bits |
| 1 kilobyte (KB) | 1,000 bytes |
| 1 megabyte (MB) | 1,000 KB |
| 1 gigabyte (GB) | 1,000 MB |
| 1 terabyte (TB) | 1,000 GB |

---

### 3.1 Numbers

#### Explanation

Binary is a **place-value** system. In everyday (decimal) numbers the places are ones, tens, hundreds. In binary the places are **powers of 2**:

| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|---|---|

To write a number in binary, put a **1** under each place value you need and a **0** under the rest.

#### Worked Example

Convert **13** to binary.

- 13 = 8 + 4 + 1
- Place values: 8 → 1, 4 → 1, 2 → 0, 1 → 1

| 8 | 4 | 2 | 1 |
|---|---|---|---|
| 1 | 1 | 0 | 1 |

**13 in binary = 1101** (or `00001101` in a full byte).

#### Activity

Convert **10** to binary.

#### Answer

10 = 8 + 2 → **1010**.

---

### 3.2 Text

#### Explanation

Computers cannot store letters directly, so every character gets a number. A **character code** is a table that links characters to numbers. A common one is **ASCII** (American Standard Code for Information Interchange). The number is then stored in binary.

| Character | ASCII number | Binary |
|---|---|---|
| A | 65 | 01000001 |
| B | 66 | 01000010 |
| a | 97 | 01100001 |

Each character uses 1 byte in basic ASCII.

#### Worked Example

Store the word **"Hi"**.

- H = 72 → `01001000`
- i = 105 → `01101001`

"Hi" = `01001000 01101001`, which is **2 bytes**.

#### Activity

1. The ASCII number for **C** is 67. Write it in binary.
2. How many bytes does the word **"CAT"** need in ASCII?

#### Answer

1. 67 = 64 + 2 + 1 → **01000011**
2. 3 characters × 1 byte = **3 bytes**.

---

### 3.3 Images

#### Explanation

A digital image is a grid of tiny squares called **pixels**. Each pixel stores a colour as a binary number.

- **Resolution:** the number of pixels (width × height).
- **Colour depth:** the number of bits used for each pixel. More bits means more possible colours.

| Colour depth | Colours possible |
|---|---|
| 1 bit | 2 (black and white) |
| 8 bits | 256 |
| 24 bits | about 16.7 million |

**File size = number of pixels × colour depth (in bits).** Divide by 8 to get bytes.

#### Worked Example

A small image is **100 × 100 pixels** with **24-bit** colour.

- Pixels: 100 × 100 = 10,000
- Bytes per pixel: 24 ÷ 8 = 3
- Size: 10,000 × 3 = **30,000 bytes = 30 KB**

#### Activity

A black-and-white (1-bit) image is **8 × 8 pixels**. How many bytes does it need?

#### Answer

8 × 8 = 64 pixels × 1 bit = 64 bits ÷ 8 = **8 bytes**.

---

### 3.4 Audio

#### Explanation

Sound is a smooth wave. To store it, the computer measures the wave many times per second. Each measurement is called a **sample**.

- **Sample rate:** how many samples are taken each second (measured in **Hz**).
- **Bit depth:** how many bits are used for each sample.

More samples and more bits give better quality, but a bigger file.

**File size = sample rate × bit depth × seconds** (in bits; divide by 8 for bytes).

#### Worked Example

One second of mono audio, **44,100 Hz**, **16 bits**:

- 44,100 × 16 = 705,600 bits
- 705,600 ÷ 8 = **88,200 bytes** (about 88 KB)

#### Activity

A voice recording uses **8,000 Hz** and **8 bits** per sample. How big is **10 seconds**?

#### Answer

8,000 × 8 × 10 = 640,000 bits ÷ 8 = 80,000 bytes = **80 KB**.

---

### 3.5 Video

#### Explanation

A video is a fast series of still images called **frames**, played together with audio.

- **Frame rate:** frames shown per second (**fps**).

A video's size grows quickly because it stores many images every second. Most videos are **compressed**, meaning the file is made smaller by removing or simplifying data, so they take far less space than the raw calculation suggests.

**Uncompressed size ≈ size of one frame × frames per second × seconds** (plus audio).

#### Worked Example

Each frame is 1 MB and the video runs at 10 fps.

- 1 second = 10 × 1 MB = 10 MB
- 3 seconds = **30 MB**

#### Activity

Each frame is 2 MB and the video runs at 5 fps. How big is **4 seconds** of uncompressed video?

#### Answer

2 MB × 5 fps × 4 s = **40 MB**.

---

## 4. Types of Data Storage (Primary and Secondary)

### 4.1 Primary Storage

#### Explanation

**Primary storage** is memory the CPU can reach directly and very quickly. It includes RAM, ROM and cache.

**RAM (Random Access Memory)**
- Holds data and programs **while the computer is running**.
- Very fast.
- **Volatile:** everything is lost when the power is off.
- Comes as modules plugged into the motherboard, such as **DDR4** or **DDR5** (types of RAM with different speeds and capacities).

**ROM (Read-Only Memory)**
- Holds data that **cannot be easily changed**.
- **Non-volatile:** keeps its data without power.
- In modern computers it usually holds **firmware**, software built into hardware that tells the device how to start up and work.

**Cache memory**
- A **smaller, faster** type of volatile memory placed **close to the CPU**.
- Stores **frequently used** information so the CPU does not have to wait for RAM.

#### Worked Example

When you switch on a laptop:

1. **ROM** provides the firmware that starts the computer.
2. The system loads into **RAM**.
3. Instructions the CPU uses again and again are kept in **cache** for speed.

#### Activity

Match each description to **RAM**, **ROM** or **Cache**:

1. Keeps the start-up firmware, even when the power is off.
2. Holds the programs you have open right now.
3. Small, very fast memory next to the CPU for frequently used data.

#### Answer

1. **ROM**
2. **RAM**
3. **Cache**

---

### 4.2 Secondary Storage

#### Explanation

**Secondary storage** is for **permanent** storage. It includes hard drives (HDD), solid-state drives (SSD), optical drives and USB flash drives.

- **Non-volatile:** data stays when the computer is off.
- **Larger capacity** than primary storage.
- **Slower** than primary storage.
- Used for documents, system files, applications and databases.

#### Primary vs Secondary at a glance

| Feature | Primary storage (RAM) | Secondary storage |
|---|---|---|
| Speed | Very fast | Slower |
| Capacity | Smaller | Much larger |
| Volatile? | Yes (RAM) | No |
| Purpose | Data in use right now | Long-term saving |
| Examples | RAM, cache, ROM | HDD, SSD, USB drive, DVD |

#### Worked Example

Why not just save everything in RAM, since it is so fast?

Because RAM needs constant power, everything would vanish when you switch off. So data that is not being used right now is **moved to secondary storage**, which is slower but keeps it safe.

#### Activity

A student has a **16 GB RAM** laptop and a **512 GB SSD**. Which one holds her photos after she shuts down the laptop, and why?

#### Answer

The **SSD**. It is secondary storage, so it is non-volatile and keeps the photos without power. RAM is volatile and would lose them.

---

## 5. Data Storage Devices (HDD, SSD, USB Drives)

### Explanation

| Device | How it works | Main points |
|---|---|---|
| **Hard Disk Drive (HDD)** | Stores data magnetically on **spinning platters** (disks). | Large capacity, traditional, has moving parts. |
| **Solid-State Drive (SSD)** | Uses **flash memory** (chips that keep data without power). | Much faster than HDD, **no moving parts**. |
| **Optical storage** | A laser reads data from discs such as **CDs, DVDs and Blu-rays**. | Used for media or backup files. |
| **USB flash drive** | A small **solid-state** device that connects through a **USB port**. | Portable; capacities from a few GB up to several TB. |

#### USB drives in more detail

USB drives are commonly used to **transfer files** between devices and for **backup**.

**Advantages**
- **Portable:** small and light, easy to carry.
- **Plug-and-play:** no installation needed. Plug it into a USB port and it is ready to use.

**Disadvantages**
- **Limited lifespan:** like all flash storage, a USB drive can only be written to a limited number of times (called **write cycles**). Most people will never reach this limit unless they use the drive heavily.
- **Easy to lose or damage:** its small size means it can be misplaced or damaged if handled carelessly.

#### Data access and retrieval

- **Primary storage (RAM)** is much faster than secondary storage, so the CPU can get data quickly. It needs a constant power supply, which is why data not in use is moved to secondary storage.
- **Secondary storage** offers more capacity and long-term storage, but at slower speeds.

### Worked Example

**Task:** A photographer needs to carry 20 GB of photos to a friend's house.

- Needs: portable, easy to use on any computer, enough capacity.
- Best choice: a **USB flash drive** (e.g. 64 GB). It is small, plug-and-play, and 64 GB is plenty.
- Why not an HDD? Less convenient to carry and has moving parts that can be damaged by knocks.

Extra check: if each photo is 4 MB, how many fit on a 64 GB drive? 64 GB = 64,000 MB, and 64,000 ÷ 4 = **16,000 photos**.

### Activity

Choose the best device for each situation and give one reason:

1. A laptop that must start up and open programs as fast as possible.
2. A cheap way to keep 4 TB of rarely used old videos at home.
3. Quickly moving a school presentation from one computer to another.
4. Distributing a film to customers on a disc.

### Answer

1. **SSD**, it is much faster and has no moving parts.
2. **HDD**, it offers large capacity at a lower cost per GB.
3. **USB flash drive**, it is portable and plug-and-play.
4. **Optical disc (DVD/Blu-ray)**, it is designed for storing and distributing media.

---

## 6. Summary and Revision Checklist

**Key points**

- **Storage** holds data so the CPU and other components can access it.
- Computers store everything as **binary** (0s and 1s). 8 bits = 1 byte.
- **Numbers** use place values (powers of 2), **text** uses character codes like ASCII, **images** use pixels, **audio** uses samples, and **video** uses frames.
- **Primary storage** (RAM, ROM, cache) is fast and close to the CPU. RAM and cache are volatile.
- **Secondary storage** (HDD, SSD, optical, USB) is slower, larger and non-volatile.
- **HDD** = spinning magnetic platters. **SSD** = flash, faster, no moving parts. **USB drive** = portable flash storage.

**Can you do these?**

- [ ] Explain the difference between volatile and non-volatile storage.
- [ ] Describe the path of data from drive to RAM to CPU and back.
- [ ] Convert a small number to binary.
- [ ] Calculate the size of a simple image or sound.
- [ ] Compare RAM, ROM and cache.
- [ ] Compare HDD, SSD, optical and USB storage and pick one for a task.
>>>>>>> origin/topic-1.1
