# Computer Basics: Data, Output, Storage, and Types of Computers

## Learning Goal

Identify the core physical components of computers and explain their basic functions.

**How each section works:** Explanation → Worked Example → Activity → Answer.
Every new term is defined the first time it appears.

---

## Stage 1 Link: Where This Fits

These notes support **Stage 1: Von Neumann Model**, specifically *Components (2): Memory, Input, and Output*. Before looking at output and storage, we first need to understand how a computer represents information.

---

## 1. How Computers Store Information (Binary)

### Explanation

A computer's hardware only understands two states: **on** and **off**.

- A **bit** (short for *binary digit*) is the smallest piece of data. It is either `1` (on / True) or `0` (off / False).
- **Binary** is a number system that uses only the digits `0` and `1`.
- A **byte** is a group of 8 bits.

Because everything in a computer is built from bits, bits can be combined to make bigger things such as:

- **Integers** – whole numbers (e.g., 5, 42)
- **Floating-point numbers** – numbers with decimals (e.g., 3.14)
- **Characters** – letters, digits, and symbols (e.g., `A`, `7`, `?`)

#### Place values

In binary, each position has a **place value**: a number that tells you how much a `1` in that position is worth. Place values double each time as you move left, and we read them from **right to left**:

| Power | 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|-------|----|----|----|----|----|----|----|----|
| Value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

To convert binary to a decimal (everyday) number: **add up the place values that have a `1`.**

### Worked Example

Convert `00010011` to decimal.

| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-------------|-----|----|----|----|---|---|---|---|
| Bit         | 0   | 0  | 0  | 1  | 0 | 0 | 1 | 1 |

Only add the columns with a `1`:

```
16 + 2 + 1 = 19
```

**Answer: `00010011` = 19**

### Activity

1. Convert `00001101` to decimal.
2. Convert `01000001` to decimal.

<details>
<summary>Answer</summary>

1. Bits with a `1`: 8, 4, and 1 → 8 + 4 + 1 = **13**
2. Bits with a `1`: 64 and 1 → 64 + 1 = **65**

</details>

---

## 2. Turning Binary into Characters (ASCII)

### Explanation

Computers need a way to turn numbers into letters and symbols. **ASCII** (American Standard Code for Information Interchange) is a code that gives every character its own number.

- The number given to a character is its **ASCII code**.
- The computer stores the code in binary, then uses it to display the character.
- Example: the capital letter `A` has the ASCII code **65**, which is `01000001` in binary.

A group of related characters is called a **character set**. It usually includes:

- **Alphanumeric data** – letters and numbers
- **Symbols** – such as `?`, `&`, `:`
- **Control characters** – special keys that do actions rather than show a picture, such as Backspace, Horizontal Tab, and Escape

#### Extended ASCII and UTF-8

- Standard ASCII uses **7 bits**, giving 2⁷ = **128** characters.
- As software spread across the world, more characters were needed (accented letters, extra symbols). **Extended ASCII** uses **8 bits** (one full byte), giving 2⁸ = **256** characters. One example is **ISO-8859-1 (Latin-1)**, which adds characters for Western European languages.
- The 8th bit was sometimes used as a **parity bit**, a simple error check. It tells the computer whether the number of `1`s in the data is odd or even, so it can spot some mistakes.
- Modern computers use **Unicode**, a huge character set that covers almost every language. **UTF-8** is the most common way to store Unicode text. It is *backward compatible* with ASCII, meaning older ASCII text still works in UTF-8.

### Worked Example

Which character does `01000010` stand for?

1. Add the place values with a `1`: 64 + 2 = **66**
2. Look up 66 in the ASCII table → **`B`**

(Check: `A` = 65, so the next letter `B` = 66 ✔)

### Activity

1. The ASCII code for `C` is 67. Write it in 8-bit binary.
2. How many different characters can 8 bits represent?

<details>
<summary>Answer</summary>

1. 67 = 64 + 2 + 1 → `01000011`
2. 2⁸ = **256** characters

</details>

---

## 3. Other Number Systems: Octal and Hexadecimal

### Explanation

A **number system** is a way of writing numbers using a set of digits. Each system has a **base**, which is how many different digits it uses before it "rolls over" to the next place (just like 9 rolls over to 10 in decimal).

| System | Base | Digits used |
|--------|------|-------------|
| Binary | 2 | 0–1 |
| Octal | 8 | 0–7 |
| Decimal | 10 | 0–9 |
| Hexadecimal | 16 | 0–9 and A–F (A=10, B=11, C=12, D=13, E=14, F=15) |

**Octal** (base 8) is a shorthand for binary, because 8 is a power of 2. Each place is worth a power of 8.

**Hexadecimal** (base 16, often called *hex*) is used a lot in computing because it writes long binary numbers in a short form. For example, a 16-bit binary number fits into just 4 hex digits. Common uses:

- Memory addresses (the "location numbers" of data in memory)
- Colour codes in web design (e.g., `#FF0000` is red)
- Machine code instructions (the low-level commands the CPU runs)

### Worked Example

**A) Octal `157` to decimal**

```
1×8² + 5×8¹ + 7×8⁰
= 64 + 40 + 7
= 111
```

**B) Hex `3F2` to decimal** (F = 15)

```
3×16² + 15×16¹ + 2×16⁰
= 768 + 240 + 2
= 1010
```

### Activity

1. Convert octal `17` to decimal.
2. Convert hex `2A` to decimal (A = 10).

<details>
<summary>Answer</summary>

1. 1×8¹ + 7×8⁰ = 8 + 7 = **15**
2. 2×16¹ + 10×16⁰ = 32 + 10 = **42**

</details>

---

## 4. Converting Between Binary and Hexadecimal

### Explanation

There are two ways to convert binary to hex.

**Method 1: Indirect.** Convert to decimal first, then convert the decimal to hex.

**Method 2: Direct (grouping).** This is faster. One hex digit equals exactly **4 bits**, so:

1. Split the binary number into groups of 4 bits, starting from the **right**.
2. If the leftmost group is short, add `0`s on the left. This does not change the value.
3. Replace each group with its hex digit using the table below.

| Hex | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
|-----|------|------|------|------|------|------|------|------|
| Binary | 0000 | 0001 | 0010 | 0011 | 0100 | 0101 | 0110 | 0111 |

| Hex | 8 | 9 | A | B | C | D | E | F |
|-----|------|------|------|------|------|------|------|------|
| Binary | 1000 | 1001 | 1010 | 1011 | 1100 | 1101 | 1110 | 1111 |

### Worked Example

**A) Indirect method:** convert `1101010` to hex.

```
Step 1 (to decimal): 64 + 32 + 0 + 8 + 0 + 2 + 0 = 106
Step 2 (to hex):     106 = 6×16 + 10  →  6 and A
```

**Answer: `6A`**

**B) Grouping method:** convert `1010101101001` to hex.

```
Original:        1010101101001
Group from right: 1 | 0101 | 0110 | 1001
Pad the left:     0001 | 0101 | 0110 | 1001
Replace groups:     1  |   5  |   6  |   9
```

**Answer: `1569`**

### Activity

1. Use grouping to convert `11010110` to hex.
2. Convert hex `2F` to binary.

<details>
<summary>Answer</summary>

1. `1101` = D and `0110` = 6 → **D6**
2. `2` = `0010` and `F` = `1111` → **00101111**

</details>

---

## 5. Output

### Explanation

**Output** is the data a computer sends out to a user or another device after it has finished processing. The output system has three main parts:

| Part | What it does |
|------|--------------|
| **Output interface** | Sends processed data from inside the computer to the outside. It includes hardware (the connection) and software called **drivers**, which are small programs that let the computer talk to a device. |
| **Output devices** | Present the results in a form people can use. |
| **Digital-to-analog conversion** | Changes digital signals into analog signals for devices that need them. |

Common output devices:

- **Monitor (display):** shows text, images, or video.
- **Printer:** makes a paper copy (a *hard copy*) of a document or image.
- **Speakers:** play sound.

**Digital vs analog:** A *digital* signal is made of separate values (1s and 0s). An *analog* signal is a smooth, continuous wave. Speakers need analog waves, so a **DAC (digital-to-analog converter)** inside the sound card changes the computer's digital audio into analog waves.

#### How a DAC works (simplified)

1. The digital input (bits) arrives.
2. A register (a tiny storage spot) holds the bits.
3. Voltage switches turn the bits into electrical levels.
4. A summing circuit adds those levels together.
5. An amplifier strengthens the signal.
6. The analog output goes to the speaker.

**How output happens overall:** Input → Process → Output. When the CPU finishes processing, it sends the result to the output subsystem, which passes it to the device to be shown, printed, or played. The format depends on the data type and the device.

### Worked Example

You press play on a song file.

1. The CPU processes the digital audio file.
2. The result goes through the output interface (and the sound driver).
3. The DAC in the sound card turns the digital data into an analog wave.
4. The speakers play the wave as sound you can hear.

### Activity

Sort these into **output device** or **not an output device**: monitor, keyboard, printer, microphone, speakers.

Then answer: why does a speaker need a DAC?

<details>
<summary>Answer</summary>

- **Output devices:** monitor, printer, speakers
- **Not output devices:** keyboard and microphone (these are *input* devices)
- Speakers play analog sound waves, but the computer holds sound as digital data. The DAC converts digital to analog so the speakers can play it.

</details>

---

## 6. Storage

### Explanation

**Storage** is the part of a computer that saves and keeps data and programs. In the von Neumann model, storage holds both the **program instructions** and the **data** those instructions use. All of it is stored in binary, so the same 1s and 0s can stand for text, images, or video.

There are two kinds:

| Type | Also called | Key idea | Example |
|------|-------------|----------|---------|
| **Primary storage** | Memory | Fast and used for short-term work. It is usually **volatile**, meaning its contents are lost when the power goes off. | RAM |
| **Secondary storage** | Long-term storage | Slower but keeps data **even when the power is off**. | Hard drive, SSD, USB drive |

### Worked Example

You are writing an essay.

- While you type, the text sits in **RAM** (primary storage) so the computer can work with it quickly.
- When you press **Save**, the essay is copied to the **SSD** (secondary storage).
- After you shut down and restart, the saved essay is still there. Anything you did *not* save is gone.

### Activity

For each item, say whether it is primary or secondary storage: (a) RAM, (b) a USB flash drive, (c) a hard drive.

Which kind keeps data when the computer is turned off?

<details>
<summary>Answer</summary>

- (a) RAM: **primary**
- (b) USB flash drive: **secondary**
- (c) hard drive: **secondary**
- **Secondary storage** keeps data when the power is off.

</details>

---

## 7. The Operating System (OS)

### Explanation

An **operating system (OS)** is the main software that manages a computer's hardware and software. It sits between the user and the hardware, and it gives programs a place to run.

It provides a **user interface (UI)** so you can interact with the computer:

- **GUI (graphical user interface):** you use windows, icons, and a mouse (e.g., Windows, macOS).
- **CLI (command-line interface):** you type text commands (e.g., a Linux terminal).

**Key functions of an OS:**

| Function | What it does |
|----------|--------------|
| Resource management | Shares the CPU, memory, storage, and input/output devices between programs without conflict. |
| Program execution | Runs programs and schedules them so each gets enough CPU time. |
| Memory management | Tracks which memory is used or free, and stops programs from interfering with each other. |
| File system management | Organizes files into folders (directories) and controls who can access them. |
| User interface | Turns your clicks and commands into actions the computer can do. |
| Device management | Helps the computer communicate with devices such as printers and drives. |
| Security | Protects users and data with tools like access controls and encryption (scrambling data so only the right people can read it). |
| Networking | Sets up and manages network connections and sharing of files. |
| Backup and recovery | Helps back up data and restore it after errors or failures. |
| System calls | A standard set of requests that programs use to ask the OS for help, which makes programs work across different hardware. |

Many modern operating systems are **multi-user** (several people can use the system) and **multitasking** (several programs run at the same time). This is important for servers and businesses.

**Common examples:**

- **Windows** (Microsoft): user-friendly and works with lots of software and hardware.
- **Linux:** known for stability, security, and being highly customizable.
- **macOS** (Apple): used on Mac computers, known for its clean design and strong creative and multimedia tools.

### Worked Example

You click **Print** in a document.

1. The program sends a *system call* asking the OS to print.
2. The OS uses **device management** and the printer driver to talk to the printer.
3. The OS uses **resource management** to keep the printing job from clashing with other running programs.
4. The printer produces the hard copy.

### Activity

Match each situation to an OS function:

1. You create a folder called "Homework" and move files into it.
2. Two programs are open and neither can read the other's memory.
3. A password is needed to open your user account.

<details>
<summary>Answer</summary>

1. **File system management**
2. **Memory management**
3. **Security**

</details>

---

## 8. Different Types of Computers

### Explanation

Computers come in many forms, built for different jobs.

**1. Personal computers**
- **Desktop:** a separate monitor, keyboard, and CPU tower. Best for staying in one place and offers high power.
- **Laptop:** the screen, keyboard, and CPU are in one portable unit. It balances power and portability.

**2. Mobile devices**
- **Smartphone:** a pocket-sized computer for calls, messages, internet, and apps.
- **Tablet:** a larger touchscreen device between a phone and a PC. Good for browsing, watching media, and light work.

**3. Servers and supercomputers**
- **Server:** a computer that provides services to other devices on a network (e.g., web hosting, databases).
- **Supercomputer:** an extremely powerful system for huge calculations, such as scientific simulations and climate modeling.

**4. Embedded systems**
- Small computers built into other objects (appliances, cars, medical equipment, industrial machines). They do one specific job, such as the **Engine Management System (EMS)** in a car.

### Worked Example

A car's EMS monitors the engine and adjusts fuel. It is built into the car, does one specific job, and is not used like a normal computer. So it is an **embedded system**.

### Activity

Name the type of computer that best fits each:

1. A computer that stores a school's website and sends pages to students' devices.
2. A system that models weather patterns across the whole planet.
3. The small computer inside a microwave.

<details>
<summary>Answer</summary>

1. **Server**
2. **Supercomputer**
3. **Embedded system**

</details>

---

## Quick Summary

- Computers store everything as **bits** (0s and 1s). Groups of 8 bits are a **byte**.
- **ASCII** gives each character a number; **Extended ASCII** and **UTF-8** support more characters.
- **Octal** and **hex** are shorthand ways to write binary. One hex digit = 4 bits.
- **Output** sends processed results to devices such as monitors, printers, and speakers. A **DAC** converts digital to analog for speakers.
- **Storage** keeps programs and data. **Primary** (RAM) is fast and temporary; **secondary** (SSD, hard drive) is long-term.
- The **operating system** manages hardware, runs programs, and gives you an interface.
- Types of computers: **personal, mobile, servers, supercomputers, embedded systems**.

## Key Terms

| Term | Meaning |
|------|---------|
| Bit | A single 0 or 1 |
| Byte | 8 bits |
| Binary | Base-2 number system (0 and 1) |
| ASCII | A code that gives characters numbers |
| Character set | A group of characters a system can use |
| Base | How many digits a number system uses |
| Hexadecimal | Base-16 number system (0–9, A–F) |
| Octal | Base-8 number system (0–7) |
| Output | Data a computer sends out after processing |
| DAC | Converts digital signals to analog |
| Primary storage | Fast, short-term memory (e.g., RAM) |
| Secondary storage | Long-term storage that keeps data without power |
| Operating system | Software that manages hardware and runs programs |
| Embedded system | A small computer built into another object |