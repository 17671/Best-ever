# Chapter 1.1: Number Systems and Data

📄 **File:** `1-1-number-systems-and-data.md`

## Chapter Overview

> This chapter introduces what a computer is and how it works, from the basic workflow of input, processing, storage, and output down to the binary data it uses. You'll study the main physical parts of a computer, number systems, and data storage.

## Learning Outcomes

By the end of this chapter, you will be able to:

- Define a computer, identify its core physical components, and explain what each one does.
- Describe the basic workflow of a computer and distinguish between types of computers.
- Convert between binary, decimal, and hexadecimal number systems.
- Explain how numbers, text, images, audio, and video are stored as binary data.
- Distinguish between primary (RAM) and secondary storage (SSD/HDD).

## Material

| Stage | Topics |
|---|---|
| **Stage 1: Computers and Data** | • Definition of a Computer<br>• The Basic Workflow of a Computer (input, processing, storage, output)<br>• Different Types of Computers |
| **Stage 2: Number Systems** | • Number System Overview<br>• Binary Number System<br>• Decimal to Binary and Binary to Decimal<br>• Hexadecimal to Binary and Binary to Hexadecimal<br>• Hexadecimal to Decimal and Decimal to Hexadecimal |
| **Stage 3: Data Storage** | • Definition<br>• How Does Data Storage Work<br>• Representing Data in Binary (numbers, text, images, audio, video)<br>• Types of Data Storage (primary and secondary)<br>• Data Storage Devices (HDD, SSD, USB drives) |
| **Stage 4: Chapter Exercise** | — |

---

# Stage 1: Computers and Data

## 1.1 Definition of a Computer

### Explanation

A **computer** is an electronic machine that takes in data, works on it by following instructions, saves it, and shows the result.

Two words appear here that we need to define right away:

- **Data** is raw facts with no meaning on their own, such as the numbers `25`, `3`, and `90`.
- **Information** is data that has been organized so it makes sense, such as "Your test score is 90 out of 100."

A computer is made of two parts:

- **Hardware** is the physical parts you can touch (screen, keyboard, chips).
- **Software** is the set of instructions (programs) that tells the hardware what to do.

#### Core physical components (hardware)

| Component | What it is | What it does |
|---|---|---|
| **CPU** (Central Processing Unit) | A small chip often called the "brain" of the computer | Follows instructions and does calculations |
| **RAM** (Random Access Memory) | Fast, temporary memory | Holds the data and programs the computer is using right now |
| **Storage** (SSD or HDD) | Permanent memory | Keeps files saved, even when the computer is off |
| **Motherboard** | The main circuit board | Connects all the parts so they can talk to each other |
| **Input devices** | Devices that send data *into* the computer (keyboard, mouse, microphone) | Let the user give commands and data |
| **Output devices** | Devices that show results *from* the computer (screen, speaker, printer) | Let the user see or hear the results |
| **Power supply** | A unit that converts wall electricity into the power the parts need | Keeps the computer running |

[insert image about the inside of a desktop computer with the CPU, RAM, storage, motherboard, and power supply labeled]

### Worked Example

**Question:** You type a letter in a word processor and press the print button. Which hardware part does each job?

| Job | Hardware part |
|---|---|
| Pressing the keys | Keyboard (input device) |
| Holding the letter while you are still typing | RAM |
| Working out which character each key press means | CPU |
| Showing the letter on the screen | Monitor (output device) |
| Saving the letter so it is still there tomorrow | Storage (SSD or HDD) |
| Producing the paper copy | Printer (output device) |

### Activity

Match each part to its job:

1. CPU
2. RAM
3. SSD
4. Microphone
5. Speaker
6. Motherboard

- **A.** Plays sound out loud
- **B.** Connects all the parts together
- **C.** Follows instructions and does calculations
- **D.** Holds data being used right now (temporary)
- **E.** Sends sound into the computer
- **F.** Keeps files saved permanently

### Answer

<details>
<summary>Click to show the answer</summary>

1 → C, 2 → D, 3 → F, 4 → E, 5 → A, 6 → B

</details>

---

## 1.2 The Basic Workflow of a Computer

### Explanation

Every computer, from a calculator to a gaming PC, follows the same four steps. This is called the **workflow** (the order in which a job is done).

1. **Input:** Data goes into the computer (typing, clicking, taking a photo).
2. **Processing:** The CPU works on the data by following instructions.
3. **Storage:** The data and results are saved, either for a short time (RAM) or for a long time (SSD/HDD).
4. **Output:** The results are shown to the user (screen, sound, printout).

```
Input  →  Processing  →  Output
              ↕
           Storage
```

[insert image about the input, processing, storage, and output workflow of a computer]

### Worked Example

**Question:** Place each step of "using a calculator app" into the workflow.

| Step | Workflow stage |
|---|---|
| You tap `7`, `+`, `5` | Input |
| The CPU adds 7 and 5 | Processing |
| The number `12` is held in memory for a moment | Storage |
| `12` appears on the screen | Output |

### Activity

A student plays a game using a game controller. Name one example of each stage:

1. Input
2. Processing
3. Storage
4. Output

### Answer

<details>
<summary>Click to show the answer</summary>

Your answers may be a little different, but good examples are:

1. **Input:** Pressing a button on the controller.
2. **Processing:** The CPU works out that the character should jump.
3. **Storage:** The game saves your level to the SSD.
4. **Output:** The character jumps on the screen and a sound plays through the speaker.

</details>

---

## 1.3 Different Types of Computers

### Explanation

Computers come in many sizes. The right type depends on the job.

| Type | What it is | Typical use |
|---|---|---|
| **Supercomputer** | The fastest and largest computers, made of thousands of CPUs working together | Weather forecasting, scientific research |
| **Mainframe** | A very large, reliable computer that many people use at once | Banks, airlines |
| **Server** | A computer that shares its data or services with other computers over a network | Websites, email, online games |
| **Personal computer (PC)** | A computer made for one person. A *desktop* stays on a desk; a *laptop* is portable | Homework, work, gaming |
| **Smartphone and tablet** | Small touchscreen computers you can carry | Calls, messages, apps |
| **Embedded computer** | A tiny computer built inside another device | Washing machines, cars, smart watches |

[insert image about different types of computers, from a supercomputer to an embedded chip]

### Worked Example

**Question:** Which type of computer is best for a bank that must handle millions of customer transactions every day and almost never go down?

**Solution:** A **mainframe**. It is built to serve many users at once and to be very reliable. A laptop is too small for the job, and a supercomputer is built for heavy calculations, not for handling many users.

### Activity

Choose the best computer type for each situation:

1. A computer that stores a website so people around the world can open it.
2. The tiny computer inside a microwave oven.
3. A computer used to predict hurricanes by doing billions of calculations.
4. A computer a student carries to class to take notes.

### Answer

<details>
<summary>Click to show the answer</summary>

1. Server
2. Embedded computer
3. Supercomputer
4. Laptop (personal computer)

</details>

---

# Stage 2: Number Systems

## 2.1 Number System Overview

### Explanation

A **number system** is a way of writing numbers using a fixed set of symbols. Computers can only work with numbers, so number systems are the base of everything a computer does.

Every number system has a **base**. The base is how many different digits the system uses.

| Number system | Base | Digits used | Where it is used |
|---|---|---|---|
| **Binary** | 2 | 0, 1 | Inside the computer, for all data and calculations |
| **Decimal** | 10 | 0 – 9 | Everyday life; numbers people type in and read |
| **Hexadecimal** (hex) | 16 | 0 – 9 and A – F | A short way to write long binary numbers (for example, colors and memory addresses) |

In hexadecimal, the letters stand for numbers: **A = 10, B = 11, C = 12, D = 13, E = 14, F = 15**.

A small note: there is also an **octal** system (base 8, digits 0 – 7), but we will focus on binary, decimal, and hexadecimal in this chapter.

To show which system a number is written in, we write the base as a small number after it. For example, `(9)₁₀` means "9 in decimal" and `(1001)₂` means "1001 in binary".

[insert image about the binary, decimal, and hexadecimal number systems side by side]

### Worked Example

**Question:** What do the digits `1010` mean in each system?

- In **decimal**, `1010` is "one thousand and ten."
- In **binary**, `1010` is only 1s and 0s, so it could be binary. (We will learn in 2.3 that it equals 10 in decimal.)
- In **hexadecimal**, `1010` is also valid, since hex uses 0 – 9 too.

This is why we write the base after the number. Without it, `1010` could mean three different values.

### Activity

For each number, say which systems it could belong to (binary, decimal, hexadecimal):

1. `1101`
2. `275`
3. `3F`
4. `FF9`

### Answer

<details>
<summary>Click to show the answer</summary>

1. `1101`: binary, decimal, or hexadecimal (it only uses 0 and 1).
2. `275`: decimal or hexadecimal (it uses digits above 1, so it cannot be binary).
3. `3F`: hexadecimal only (the letter F is not used in binary or decimal).
4. `FF9`: hexadecimal only.

</details>

---

## 2.2 Binary Number System

### Explanation

The **binary number system** uses only two digits, **0** and **1**. Each binary digit is called a **bit** (short for "binary digit"). A group of **8 bits** is called a **byte**.

Computers use binary because their parts only have two states: **off (0)** and **on (1)**, like a light switch.

To read a binary number, we need two ideas:

- **Digit value:** the digit itself. In binary, this is only 0 or 1.
- **Place value:** how much a position is worth. In binary, place values are powers of 2, starting from the right.

| Place | 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|---|---|---|---|---|---|---|---|---|
| **Place value** | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

(A **power of 2** means 2 multiplied by itself. For example, 2³ = 2 × 2 × 2 = 8.)

[insert image about binary digit value and place value, showing the 8-bit place value chart]

### Worked Example

**Question:** What is the decimal value of `00001001`?

**Step 1:** Write the bits above the place values.

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 1 | 0 | 0 | 1 |

**Step 2:** Multiply each digit by its place value and add.

(0×128) + (0×64) + (0×32) + (0×16) + (1×8) + (0×4) + (0×2) + (1×1) = 8 + 1 = **9**

So `(00001001)₂ = (9)₁₀`.

### Activity

1. Write the place values for an 8-bit number from left to right.
2. How many bits are in one byte?
3. Why do computers use binary?

### Answer

<details>
<summary>Click to show the answer</summary>

1. 128, 64, 32, 16, 8, 4, 2, 1
2. 8 bits
3. Computer parts only have two states, off (0) and on (1), so binary is the easiest and most reliable way to store and process data.

</details>

---

## 2.3 Decimal to Binary and Binary to Decimal

### Explanation

#### Binary to decimal

Multiply each bit by its place value, then add the results. Bits that are 0 add nothing, so you can just add the place values where there is a 1.

#### Decimal to binary

There are two methods. Both give the same answer.

**Method 1: Subtract place values**

1. Write the place values (128, 64, 32, 16, 8, 4, 2, 1).
2. Find the largest place value that fits into your number. Put a **1** there and subtract it.
3. Repeat with what is left. Put a **0** in every place value you skip.
4. Stop when the remainder is 0.

**Method 2: Divide by 2**

1. Divide the number by 2. Write down the **remainder** (what is left over, either 0 or 1).
2. Divide the answer (the **quotient**) by 2 again. Write down the remainder.
3. Keep going until the quotient is 0.
4. Read the remainders from **bottom to top**.

Two more terms to know:

- **LSB (Least Significant Bit):** the bit on the far right. It is worth the least (1).
- **MSB (Most Significant Bit):** the bit on the far left. It is worth the most.

In Method 2, the first remainder you get is the LSB and the last remainder is the MSB.

[insert image about the place value table used for decimal to binary conversion]

### Worked Example

**Part A: Binary to decimal.** Convert `1101` to decimal.

| 8 | 4 | 2 | 1 |
|---|---|---|---|
| 1 | 1 | 0 | 1 |

(1×8) + (1×4) + (0×2) + (1×1) = 8 + 4 + 0 + 1 = **13**

**Part B: Decimal to binary.** Convert 9 to binary.

*Method 1 (subtract):*

- The biggest place value that fits into 9 is **8**. Put a 1 under 8. 9 − 8 = 1.
- The biggest place value that fits into 1 is **1**. Put a 1 under 1. 1 − 1 = 0.
- All other places get 0.

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 1 | 0 | 0 | 1 |

Answer: **00001001**

*Method 2 (divide by 2):*

| Division | Quotient | Remainder |
|---|---|---|
| 9 ÷ 2 | 4 | **1** ← LSB |
| 4 ÷ 2 | 2 | **0** |
| 2 ÷ 2 | 1 | **0** |
| 1 ÷ 2 | 0 | **1** ← MSB |

Read the remainders from bottom to top: **1001** (which is 00001001 with leading zeros removed).

### Activity

1. Convert `10110` (binary) to decimal.
2. Convert `11111111` (binary) to decimal.
3. Convert 13 (decimal) to binary using the divide-by-2 method.
4. Convert 20 (decimal) to binary using the subtract method.

### Answer

<details>
<summary>Click to show the answer</summary>

1. `10110` = 16 + 4 + 2 = **22**
2. `11111111` = 128 + 64 + 32 + 16 + 8 + 4 + 2 + 1 = **255**
3. 13 ÷ 2 = 6 r **1**; 6 ÷ 2 = 3 r **0**; 3 ÷ 2 = 1 r **1**; 1 ÷ 2 = 0 r **1**. Read from bottom to top: **1101**
4. The biggest place value that fits into 20 is 16 (20 − 16 = 4). Then 4 fits (4 − 4 = 0). So the 16 and 4 places get a 1: **10100**

</details>

---

## 2.4 Hexadecimal to Binary and Binary to Hexadecimal

### Explanation

**Hexadecimal** is useful because it is a short way to write long binary numbers. The key fact is:

> **One hex digit = exactly four bits.**

Four bits are sometimes called a **nibble** (half a byte). Use this table to convert quickly:

| Hex | Binary | Decimal | | Hex | Binary | Decimal |
|---|---|---|---|---|---|---|
| 0 | 0000 | 0 | | 8 | 1000 | 8 |
| 1 | 0001 | 1 | | 9 | 1001 | 9 |
| 2 | 0010 | 2 | | A | 1010 | 10 |
| 3 | 0011 | 3 | | B | 1011 | 11 |
| 4 | 0100 | 4 | | C | 1100 | 12 |
| 5 | 0101 | 5 | | D | 1101 | 13 |
| 6 | 0110 | 6 | | E | 1110 | 14 |
| 7 | 0111 | 7 | | F | 1111 | 15 |

**Hex to binary:** Replace each hex digit with its 4-bit group.

**Binary to hex:**

1. Split the binary number into groups of 4, starting from the **right**.
2. If the leftmost group has fewer than 4 bits, add **0s on the left** to fill it.
3. Replace each group with its hex digit.

[insert image about the hexadecimal to binary conversion table]

### Worked Example

**Part A: Hex to binary.** Convert `(FC)₁₆` to binary.

- F = 15 = `1111`
- C = 12 = `1100`

So `(FC)₁₆ = (11111100)₂`.

**Part B: Binary to hex.** Convert `(110011)₂` to hex.

**Step 1:** Split into groups of 4 from the right: `11` and `0011`.

**Step 2:** The left group has only 2 bits, so add 0s on the left: `0011` and `0011`.

**Step 3:** Convert each group: `0011` = 3 and `0011` = 3.

So `(110011)₂ = (33)₁₆`.

### Activity

1. Convert `(2A)₁₆` to binary.
2. Convert `(B7)₁₆` to binary.
3. Convert `(10111101)₂` to hex.
4. Convert `(1111010)₂` to hex.

### Answer

<details>
<summary>Click to show the answer</summary>

1. 2 = `0010`, A = `1010`, so `(2A)₁₆ = (00101010)₂`
2. B = `1011`, 7 = `0111`, so `(B7)₁₆ = (10110111)₂`
3. `1011` = B and `1101` = D, so `(10111101)₂ = (BD)₁₆`
4. Split from the right: `111` and `1010`. Add a 0 on the left of the first group: `0111` = 7, `1010` = A. So `(1111010)₂ = (7A)₁₆`

</details>

---

## 2.5 Hexadecimal to Decimal and Decimal to Hexadecimal

### Explanation

#### Hex to decimal

In hex, the place values are **powers of 16** instead of powers of 2:

| Place | 16² | 16¹ | 16⁰ |
|---|---|---|---|
| **Place value** | 256 | 16 | 1 |

Change any letters into numbers (A = 10 … F = 15), multiply each digit by its place value, then add.

#### Decimal to hex

1. Divide the number by 16. Write down the remainder.
2. Divide the quotient by 16 again. Write down the remainder.
3. Repeat until the quotient is 0.
4. Read the remainders from **bottom to top**. Change any remainders from 10 – 15 into the letters A – F.

[insert image about the powers of 16 place value chart]

### Worked Example

**Part A: Hex to decimal.** Convert `(12)₁₆` to decimal.

(1 × 16¹) + (2 × 16⁰) = 16 + 2 = **18**

**Part B: Decimal to hex.** Convert 127 to hex.

| Division | Quotient | Remainder |
|---|---|---|
| 127 ÷ 16 | 7 | **15** (= F) |
| 7 ÷ 16 | 0 | **7** |

Read from bottom to top: 7, then F. So `127₁₀ = (7F)₁₆`.

### Activity

1. Convert `(1A)₁₆` to decimal.
2. Convert `(2F)₁₆` to decimal.
3. Convert 45 (decimal) to hex.
4. Convert 200 (decimal) to hex.

### Answer

<details>
<summary>Click to show the answer</summary>

1. (1 × 16) + (10 × 1) = 16 + 10 = **26**
2. (2 × 16) + (15 × 1) = 32 + 15 = **47**
3. 45 ÷ 16 = 2 r **13** (D); 2 ÷ 16 = 0 r **2**. Read from bottom to top: **2D**
4. 200 ÷ 16 = 12 r **8**; 12 ÷ 16 = 0 r **12** (C). Read from bottom to top: **C8**

</details>

---

# Stage 3: Data Storage

## 3.1 Definition

### Explanation

**Data storage** means keeping data in a computer so that it can be used later.

Think of a big notebook where you write down your favorite games, pictures, and homework. Data storage is like that notebook, but for computers. Instead of paper, computers use special devices, like hard drives or USB sticks, to save the information they need. Just like your notebook keeps your drawings safe, data storage keeps the computer's files, pictures, and games safe so you can look at them again later.

[insert image about a notebook compared to a computer storage device]

### Worked Example

**Question:** You finish your homework on a laptop, shut it down, and open it again tomorrow. Why is the homework still there?

**Solution:** When you pressed "Save," the file was written to the computer's **storage** (an SSD or HDD). Storage keeps data even when the power is off, so the file is still there tomorrow.

### Activity

Which of these is an example of data storage? Explain why.

- **A.** A USB stick holding your photos
- **B.** The screen showing a video
- **C.** A keyboard

### Answer

<details>
<summary>Click to show the answer</summary>

**A.** A USB stick keeps your photos saved. The screen (B) is an output device and the keyboard (C) is an input device, so neither one stores data.

</details>

---

## 3.2 How Does Data Storage Work

### Explanation

A computer does not keep all its data in one place. It uses different kinds of storage that trade off **speed** and **permanence** (how long the data stays).

- Some storage is very fast, but it forgets everything when the power is turned off. This is called **volatile** memory. RAM is volatile.
- Other storage is a bit slower, but it keeps data for a long time, even when the computer is off. This is called **non-volatile** memory. Hard drives, SSDs, and USB drives are non-volatile.

The closer the storage is to the CPU, the faster it is, but the smaller and more temporary it is.

| Level | Example | Speed | Permanent? |
|---|---|---|---|
| 1 (closest to the CPU) | **Cache** (a tiny, very fast memory inside or next to the CPU) | Fastest | No |
| 2 | **RAM** | Very fast | No |
| 3 | **Storage devices** (SSD, HDD, USB drive) | Slower | Yes |

**Cloud storage** works like a magical notebook kept on the internet. You can open your files from any computer or phone as long as you are connected to the internet, and your files stay safe even if you don't have your own computer with you.

[insert image about the memory hierarchy, showing the CPU, cache, RAM, and permanent storage]

### Worked Example

**Question:** You are writing an essay and the power suddenly goes out. You did not press save. What happens to the essay?

**Solution:** The essay was only in **RAM**, which is volatile. When the power went off, RAM was cleared and the essay was lost. If you had pressed "Save," a copy would have been written to the SSD or HDD, which is non-volatile, and it would have survived.

### Activity

1. Is RAM volatile or non-volatile?
2. Put these in order from fastest to slowest: SSD, Cache, RAM.
3. Name one benefit of cloud storage.

### Answer

<details>
<summary>Click to show the answer</summary>

1. Volatile. It loses its data when the power is off.
2. Cache → RAM → SSD
3. You can reach your files from any device with an internet connection. (Another correct answer: your files are not tied to just one device.)

</details>

---

## 3.3 Representing Data in Binary

### Explanation

Computers only understand 0s and 1s, so every type of data must be turned into binary first. This is called **encoding**.

#### Storage units

We need names for how much data we have:

| Unit | Size |
|---|---|
| **Bit** | A single 0 or 1 |
| **Byte** | 8 bits |
| **Kilobyte (KB)** | about 1,000 bytes |
| **Megabyte (MB)** | about 1,000 KB |
| **Gigabyte (GB)** | about 1,000 MB |
| **Terabyte (TB)** | about 1,000 GB |

(Some systems use 1,024 instead of 1,000. We will use 1,000 to keep the math simple.)

#### How each type of data is stored

| Data type | How it is stored in binary |
|---|---|
| **Numbers** | Converted straight to binary (as in Stage 2). |
| **Text** | Each character gets a number from a code table. A common table is **ASCII**. For example, `A` = 65, which is `01000001` in binary. |
| **Images** | A picture is a grid of tiny dots called **pixels**. Each pixel's color is stored as a number. In many systems, a color is made from three numbers (red, green, blue). Hex is often used to write them, such as `#FF0000` for pure red. |
| **Audio** | Sound is a smooth wave. The computer measures the height of the wave many times per second (this is called **sampling**) and stores each measurement as a binary number. |
| **Video** | A video is a fast series of still images (called **frames**) plus an audio track. Each frame is stored like an image. |

[insert image about how text, images, audio, and video are converted into binary]

### Worked Example

**Question:** How is the word `Hi` stored in ASCII?

**Step 1:** Look up each letter's ASCII number. `H` = 72 and `i` = 105.

**Step 2:** Convert each number to binary (8 bits).

- 72 = 64 + 8 → `01001000`
- 105 = 64 + 32 + 8 + 1 → `01101001`

So `Hi` is stored as `01001000 01101001`. That is 2 bytes.

### Activity

1. The ASCII number for `C` is 67. Write `C` in 8-bit binary.
2. How many bits are in 3 bytes?
3. A photo is 3 MB. How many of these photos fit on a 12 GB phone? (Use 1 GB = 1,000 MB.)
4. What is a pixel?

### Answer

<details>
<summary>Click to show the answer</summary>

1. 67 = 64 + 2 + 1 → **01000011**
2. 3 × 8 = **24 bits**
3. 12 GB = 12,000 MB. 12,000 ÷ 3 = **4,000 photos**
4. A pixel is one tiny dot of color in an image. A picture is made of a grid of many pixels.

</details>

---

## 3.4 Types of Data Storage

### Explanation

Storage is grouped into three types, based on how fast it is and how long it keeps data.

| | **Primary storage** | **Secondary storage** | **Tertiary storage** |
|---|---|---|---|
| **Also called** | Main memory | Permanent storage | Archive storage |
| **Speed** | Fast, directly accessed by the CPU | Slower than primary | Slowest |
| **Keeps data when power is off?** | Usually no (RAM), but ROM does | Yes | Yes |
| **Capacity (size)** | Smaller | Larger than primary | Very large |
| **Examples** | RAM, ROM | HDD, SSD, optical discs, USB drives | Magnetic tape, cloud "cold" storage |
| **Typical use** | Running programs right now | Saving files and programs | Long-term backups that are rarely opened |

Two kinds of primary memory:

- **RAM (Random Access Memory):** volatile. Holds data while the device is on.
- **ROM (Read-Only Memory):** non-volatile. Holds permanent start-up instructions (called **firmware**) that the computer needs to switch on.

[insert image about primary, secondary, and tertiary storage examples]

### Worked Example

**Question:** Is a USB drive primary or secondary storage?

**Solution:** **Secondary.** It keeps data when unplugged or powered off, it has a larger capacity than RAM, and it is slower than RAM. All three match secondary storage.

### Activity

Classify each as primary, secondary, or tertiary storage:

1. RAM
2. SSD
3. A magnetic tape in a company's backup room
4. A Blu-ray disc

### Answer

<details>
<summary>Click to show the answer</summary>

1. Primary
2. Secondary
3. Tertiary
4. Secondary (optical disc)

</details>

---

## 3.5 Data Storage Devices (HDD, SSD, USB Drives)

### Explanation

| Device | How it works | Pros | Cons |
|---|---|---|---|
| **HDD** (Hard Disk Drive) | Stores data on spinning metal disks using magnetism | Large capacity, low cost | Slower; has moving parts that can break |
| **SSD** (Solid State Drive) | Stores data in **flash memory** chips (memory with no moving parts) | Faster, quieter, more durable | Costs more per GB |
| **USB drive** | A small portable flash memory stick that plugs into a USB port | Small and easy to carry | Easy to lose; smaller capacity |
| **Optical disc** (CD, DVD, Blu-ray) | Data is read from the disc with a laser | Cheap; good for media and backups | Slow; can be scratched |

[insert image about an HDD, an SSD, and a USB drive side by side]

#### Useful storage ideas

| Term | Meaning |
|---|---|
| **Capacity** | How much data a device can hold (measured in GB or TB) |
| **Access speed** | How fast data can be read or written |
| **Durability** | How well the device keeps data safe over time without damage |
| **Scalability** | How easily you can add more space (cloud storage is easy to scale) |

#### Cloud storage

**Cloud storage** means saving your data in a data center owned by another company and reaching it over the internet. You can open your files on any device. The company looks after the servers, but **you** are still responsible for looking after your own data (for example, using a strong password).

[insert image about how cloud storage works, with a client computer, a control node, and several storage servers]

Cloud storage can be organized in three ways:

| Form | How it works | Best for |
|---|---|---|
| **File storage** | Data is saved as files inside folders, like on your own computer | Everyday documents |
| **Block storage** | Data is split into fixed-size pieces called blocks, each with its own ID | Databases that need speed |
| **Object storage** | Data is saved as objects, each with an ID and **metadata** (information that describes the data, such as its date and type) | Photos, videos, and backups |

[insert image about block, file, and object storage]

#### Keeping data safe

- **Backup:** a spare copy of your data in case the original is lost or damaged. Keep it on an external drive or in the cloud.
- **Encryption:** scrambling data so only people with the right key can read it.
- **Access control:** deciding who is allowed to open or change the data (using accounts and passwords).
- **Data integrity:** making sure data stays correct and has not been changed by mistake.

### Worked Example

**Question:** A school wants to store 10 years of old exam papers. They rarely need them, but must not lose them. Which device or storage type would work well, and why?

**Solution:** An **HDD** or **cloud storage** is a good fit. HDDs offer large capacity at low cost, and speed is not important because the files are rarely opened. The school should also keep a **backup** copy in a second place so one failure does not lose everything.

### Activity

1. Which is faster, an HDD or an SSD?
2. Why does an SSD handle being dropped better than an HDD?
3. What is a backup, and why is it useful?
4. In cloud storage, who looks after the servers, and who looks after the data?

### Answer

<details>
<summary>Click to show the answer</summary>

1. The SSD is faster.
2. An SSD has no moving parts. An HDD has spinning disks that can be damaged by a drop.
3. A backup is a spare copy of your data. It is useful because you can restore your files if the original is lost, damaged, or deleted.
4. The cloud company looks after the servers. The user (data owner) looks after their own data.

</details>

---

# Stage 4: Chapter Exercise

Try these on your own first, then check the answers.

### Part A: Computer components

1. Name the four steps of the computer workflow, in order.
2. Which component is called the "brain" of the computer?
3. Is a printer an input device or an output device?
4. Which type of computer is built inside a washing machine?

### Part B: Number systems

5. Convert `(10011)₂` to decimal.
6. Convert 25 (decimal) to binary.
7. Convert `(3C)₁₆` to binary.
8. Convert `(11010110)₂` to hex.
9. Convert `(5B)₁₆` to decimal.
10. Convert 90 (decimal) to hex.

### Part C: Data and storage

11. How many bits are in 1 byte?
12. Which type of memory loses its data when the power is turned off: RAM or SSD?
13. Name two differences between an HDD and an SSD.
14. Explain in one or two sentences how a picture is stored as binary.
15. Is a Blu-ray disc primary, secondary, or tertiary storage?

### Answers

<details>
<summary>Click to show the answers</summary>

**Part A**

1. Input → Processing → Storage → Output
2. The CPU
3. Output device
4. Embedded computer

**Part B**

5. 16 + 2 + 1 = **19**
6. 25 = 16 + 8 + 1 → **11001**
7. 3 = `0011`, C = `1100` → **00111100**
8. `1101` = D, `0110` = 6 → **D6**
9. (5 × 16) + 11 = 80 + 11 = **91**
10. 90 ÷ 16 = 5 r **10** (A); 5 ÷ 16 = 0 r **5** → **5A**

**Part C**

11. 8 bits
12. RAM
13. Any two of: an SSD is faster; an SSD has no moving parts and is more durable; an SSD usually costs more per GB; an HDD usually offers more capacity for the price.
14. A picture is a grid of tiny pixels. The color of each pixel is stored as a number, and every number is saved in binary.
15. Secondary storage (optical disc)

</details>

---

## Chapter Summary

- A **computer** takes **input**, **processes** it, **stores** data, and gives **output**. Its core physical parts include the CPU, RAM, storage, motherboard, input devices, output devices, and power supply.
- Computers use **binary** (base 2). **Hexadecimal** (base 16) is a short way to write binary, since 1 hex digit = 4 bits.
- To convert between systems, use **place values** (multiplying and adding) or **repeated division** (reading the remainders from bottom to top).
- All data (numbers, text, images, audio, and video) is stored as binary.
- **Primary storage** (RAM) is fast but temporary. **Secondary storage** (SSD, HDD, USB) is slower but permanent.
