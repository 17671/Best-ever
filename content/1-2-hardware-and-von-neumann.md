# Stage 1: Von Neumann Model

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions.
2. Describe the von Neumann model and why it matters.
3. Explain the fetch-decode-execute process.
4. Describe the CPU and its two parts, the control unit and the ALU.
5. Explain the roles of memory, input, and output.

**Topics covered:**

- Definition
- Process (fetch-decode-execute)
- Components (1): CPU (control unit and ALU)
- Components (2): Memory, Input, and Output

---

# 1.1 Definition

## Explanation

Early computers had a big problem. Every time they needed to do a new job, people had to **rewire** them by hand. This took a long time.

Around 1944–1945, a mathematician named **John von Neumann** came up with a better idea. He noticed that **programs and data are really the same kind of thing: information**. (A **program** is a list of instructions that tells the computer what to do, and **data** is the information the program works on.) So, he suggested that a program should be **stored in the computer's memory**, right next to the data it uses.

This idea created the **von Neumann model**, which is the base of **most modern computers**.

The model divides a computer into **four subsystems**. A **subsystem** is a smaller part that does one main job within the whole computer.

| Subsystem | Its job |
|-----------|---------|
| **Memory** | Stores both programs and data |
| **Arithmetic Logic Unit (ALU)** | Performs calculations and logic operations |
| **Control Unit** | Manages all the operations |
| **Input/Output** | Handles the exchange of data with the outside world |

The big benefit: because the program and data sit in the **same memory**, a computer can **switch easily between tasks**, without anyone needing to rewire the machine.

[insert image about the von Neumann model: Input data enters Input/Output, which connects to the ALU, Memory, and Control Unit, and Output data leaves]

## Worked Example

**Task:** Explain how a computer changes from playing music to editing a document.

| Old way (before von Neumann) | Von Neumann way |
|------------------------------|-----------------|
| Engineers rewire the machine for the new job | The new program is loaded into memory |
| Slow and difficult | Fast and easy |

In the von Neumann model, the computer simply loads the document-editing program into memory, and the control unit starts following its instructions.

## Activity

a. What big idea did von Neumann add to computer design?
b. Name the four subsystems of the von Neumann model.
c. Why does storing programs in memory make switching tasks easier?

<details>
<summary><b>Answer</b></summary>

a. Programs should be **stored in the computer's memory**, together with the data.
b. **Memory, Arithmetic Logic Unit (ALU), Control Unit, and Input/Output.**
c. To change tasks, the computer just loads a different program into memory. No one has to **rewire** the machine.

</details>

---

# 1.2 Process: Fetch-Decode-Execute

## Explanation

In the von Neumann model, the computer follows its program **one instruction at a time, in order**. This keeps programs running in an organized and predictable way. (An **instruction** is a single step the computer can carry out, such as "add these two numbers".)

For each instruction, the computer repeats a three-step cycle called the **fetch-decode-execute cycle**:

| Step | What happens | Who does it |
|------|--------------|-------------|
| **1. Fetch** | The next instruction is **fetched** (brought) from memory | Control unit |
| **2. Decode** | The instruction is **decoded**, which means its meaning is worked out and the right parts are told what to do | Control unit |
| **3. Execute** | The instruction is **executed** (carried out) | ALU, or another part such as input/output |

After the execute step, the computer moves on to the **next instruction** and the cycle starts again. The computer remembers where it is in the program using a small storage spot called the **program counter**. The program counter holds the **address** (the location number in memory) of the next instruction.

[insert image about the fetch-decode-execute cycle as a loop between memory, control unit, and ALU]

## Worked Example

**Task:** A program in memory has two instructions:

1. Add 4 and 6, and store the result.
2. Output the result.

| Cycle | Step | What happens |
|-------|------|--------------|
| 1 | Fetch | The control unit gets "Add 4 and 6" from memory |
| 1 | Decode | The control unit works out that this means "add" and tells the ALU |
| 1 | Execute | The ALU calculates 4 + 6 = 10, and the result is stored in memory |
| 2 | Fetch | The program counter moves on, and the control unit gets "Output the result" |
| 2 | Decode | The control unit works out that this means "send to the screen" |
| 2 | Execute | The output part displays **10** on the screen |

## Activity

a. Put these steps in the correct order: **Execute**, **Fetch**, **Decode**.
b. Which step brings an instruction from memory to the control unit?
c. What does the program counter keep track of?

<details>
<summary><b>Answer</b></summary>

a. **Fetch → Decode → Execute**
b. **Fetch**
c. The **address of the next instruction** to run.

</details>

---

# 1.3 Components (1): The CPU (Control Unit and ALU)

## Explanation

The **Central Processing Unit (CPU)** is the "brain" of the computer. It is the part that **processes** data and carries out instructions. The CPU is made of **two main parts**:

- **Control Unit**
- **Arithmetic Logic Unit (ALU)**

### Control Unit

The **control unit** **manages all the operations** in the computer. You can think of it as a **traffic controller** or a **manager**. It does not do the calculations itself. Instead, it:

- **Fetches** instructions from memory.
- **Decodes** them to understand what they mean.
- **Tells the other parts** (ALU, memory, input/output) what to do and when.

### Arithmetic Logic Unit (ALU)

The **ALU** is the part that does the **actual calculations and comparisons**. It performs two kinds of operations:

| Kind | Meaning | Examples |
|------|---------|----------|
| **Arithmetic operations** | Math on numbers | Add, subtract, multiply, divide |
| **Logic operations** | Comparing values and making true/false decisions | Is 15 greater than 12? Are these two numbers equal? |

So: **CPU = Control Unit + ALU**.

[insert image about the CPU containing the control unit and the ALU]

## Worked Example

**Task:** The program says: "If the player's score is more than 100, show 'You win!'" The score is 120.

| Step | Part | What happens |
|------|------|--------------|
| 1 | Control unit | Fetches and decodes the instruction "compare score with 100" |
| 2 | Control unit | Sends the numbers 120 and 100 to the ALU |
| 3 | ALU | Performs a **logic operation**: is 120 > 100? The answer is **True** |
| 4 | Control unit | Sees the answer is True and tells the output part to show "You win!" |

## Activity

Decide whether each job belongs to the **control unit** or the **ALU**:

a. Calculating 25 + 17
b. Deciding which instruction to run next
c. Checking whether two numbers are equal
d. Telling the memory to send an instruction

<details>
<summary><b>Answer</b></summary>

a. **ALU** (arithmetic operation)
b. **Control unit**
c. **ALU** (logic operation)
d. **Control unit**

</details>

---

# 1.4 Components (2): Memory, Input, and Output

## Explanation

The other two subsystems of the von Neumann model are **memory** and **input/output**. Together with the CPU, they make up the computer's **hardware**.

**Hardware** means the **physical components** of a computer, the parts you can touch. The memory, the ALU, and the input/output parts are all hardware.

### Memory

**Memory** is where the computer stores **both programs and data**, in the **same place**. Each location in memory has its own **address**, like a house number, so the control unit can find exactly the instruction or data it needs.

[insert image about memory holding Program and Data together, with address numbers]

### Input

**Input** is the **data or commands that the computer receives** from users or devices. Examples: typing on a keyboard, moving a mouse, or speaking into a microphone.

### Output

**Output** is the **result that the computer gives back** to the user. Examples: showing text on a screen (a display) or printing a page on a printer.

Together, **input and output let the user and the computer interact** with each other. In the von Neumann model, both are handled by the **Input/Output subsystem**.

| Component | Main job | Example |
|-----------|----------|---------|
| **Memory** | Stores programs and data | The chips that hold your open apps |
| **Input** | Brings data into the computer | Keyboard, mouse, microphone |
| **Output** | Sends results out to the user | Screen, printer, speakers |

[insert image about an input example: a keyboard sending data to the computer screen]

[insert image about an output example: the computer sending a document to a printer]

## Worked Example

**Task:** You type `5 + 3` into a calculator program and see the answer on the screen. Show how all four subsystems work together.

| Step | Subsystem | What happens |
|------|-----------|--------------|
| 1 | **Input** | You type `5 + 3` on the keyboard, and the computer receives it |
| 2 | **Memory** | The numbers 5 and 3 and the "add" instruction are stored in memory |
| 3 | **Control unit** | Fetches and decodes the "add" instruction |
| 4 | **ALU** | Calculates 5 + 3 = 8 |
| 5 | **Memory** | Stores the result, 8 |
| 6 | **Output** | Displays **8** on the screen |

## Activity

a. What is **hardware**?
b. Which subsystem stores both programs and data?
c. Name one input device and one output device.
d. Put these steps in order for printing a typed letter: **Printer produces the page**, **You type the letter**, **The CPU processes the text**.

<details>
<summary><b>Answer</b></summary>

a. The **physical components** of a computer, such as memory, the ALU, and the input/output parts.
b. **Memory**
c. For example, input device: **keyboard** (or mouse or microphone). Output device: **printer** (or screen or speakers).
d. **You type the letter → The CPU processes the text → The printer produces the page**

</details>

---

## Stage 1 Summary

- The **von Neumann model** says that programs and data are both information, so they can be **stored together in memory**. This lets computers switch tasks easily without being rewired.
- The model has four subsystems: **Memory**, **ALU**, **Control Unit**, and **Input/Output**.
- The computer follows instructions one at a time using the **fetch-decode-execute cycle**: fetch the instruction from memory, decode what it means, and execute it.
- The **CPU** is made of the **control unit** (the manager that directs everything) and the **ALU** (which does arithmetic and logic operations).
- **Memory** stores programs and data. **Input** brings data in, and **output** gives results back to the user.
- **Hardware** is the physical part of a computer.

# Stage 1: Von Neumann Model (Input and the Processing Unit)

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions.
2. Describe how the von Neumann model handles input and processing.
3. Explain the steps the processing unit follows when it receives input.
4. Describe the CPU and its two parts, the control unit and the ALU.
5. Identify input controllers, input devices, and input data, and explain how they work with memory and output.

**Topics covered:**

- Definition
- Process (fetch-decode-execute)
- Components (1): CPU (control unit and ALU)
- Components (2): Memory, Input, and Output

---

# 1.1 Definition

## Explanation

The **von Neumann model** describes a computer as four **subsystems** (smaller parts that each do one main job):

| Subsystem | Its job |
|-----------|---------|
| **Memory** | Stores both programs and data |
| **Arithmetic Logic Unit (ALU)** | Performs calculations and logic operations |
| **Control Unit** | Manages all operations |
| **Input/Output** | Moves data between the computer and the outside world |

In this stage, we look closely at two things that happen first when you use a computer:

1. **Input**: Data enters the computer. (**Input** means the data or commands a computer receives from users or devices.)
2. **Processing**: The computer works on that data. This is done by the **processing unit**, which is usually the **Central Processing Unit (CPU)**. The CPU is the "brain" of the computer, and it is made of the **control unit** and the **ALU**.

An **input system** has four elements that work together as a chain:

| Element | Job |
|---------|-----|
| **Input interface** | Gathers data from outside and delivers it to the computer (for example, a USB port) |
| **Input controller** | Receives signals from the input device, prepares the data, and passes it to the CPU |
| **Input device** | The tool the user touches or speaks to, such as a keyboard or microphone |
| **Input data** | The actual information being sent in |

Then the **processing unit** takes over and works on the data.

[insert image about the path of data: input device, input controller, input interface, then the CPU]

## Worked Example

**Task:** Follow a mouse click through the system.

| Step | Part | What happens |
|------|------|--------------|
| 1 | Input device | You click the mouse |
| 2 | Input controller | The click signal is picked up and prepared |
| 3 | Input interface | The USB port carries it to the computer |
| 4 | Processing unit (CPU) | The CPU works out what the click means and acts on it |

## Activity

Put these parts in the order that data passes through them when you press a key: **CPU**, **keyboard**, **input controller**.

<details>
<summary><b>Answer</b></summary>

**Keyboard → Input controller → CPU**

(The keyboard is where the data starts, the controller prepares it, and the CPU processes it.)

</details>

---

# 1.2 Process (Fetch-Decode-Execute)

## Explanation

Once the input arrives, the **processing unit** (usually the CPU) has the job of **interpreting** (understanding) and **executing** (carrying out) the instructions that come with the input.

The processing unit does three things:

| Job | What it means |
|-----|---------------|
| **Analyzes** | Looks at the data and **converts it into a format the system can use** (binary) |
| **Executes** | Carries out the **operations** the input asks for |
| **Communicates** | Works with other components, such as **memory**, **storage**, and **output devices**, to complete bigger tasks |

All data inside a computer is **binary**, which means it is written using only `0` and `1`. So the processing unit always converts input into binary first.

This fits with the **fetch-decode-execute cycle** of the von Neumann model, where the computer repeats three steps for each instruction:

1. **Fetch**: Get the next instruction from memory.
2. **Decode**: Work out what the instruction means.
3. **Execute**: Carry it out.

[insert image about the processing unit's three jobs: analyze, execute, communicate]

## Worked Example

**Task:** You press the key **A** on a keyboard. What happens?

| Step | What the processing unit does | Job |
|------|-------------------------------|-----|
| 1 | Recognizes that a key was pressed | Analyzes |
| 2 | Converts the key press into binary code. The letter `A` has the ASCII number 65, which is `01000001` in binary | Analyzes |
| 3 | Triggers the action: "show the letter A" | Executes |
| 4 | Sends the letter to the screen through the output system, and may save it in memory | Communicates |

Result: the letter **A** appears on your screen.

## Activity

You press the key `B` on the keyboard. The ASCII number for `B` is 66.

a. Which of the three jobs (analyze, execute, communicate) covers converting the key press into binary?
b. Which job covers sending the letter to the screen?
c. What is the binary code for 66? (Hint: 64 + 2.)

<details>
<summary><b>Answer</b></summary>

a. **Analyze**
b. **Communicate** (the processing unit works with the output devices). The action that makes the letter appear is the **execute** job.
c. 64 + 2 = 66, so the binary code is **01000010**.

</details>

---

# 1.3 Components (1): CPU (Control Unit and ALU)

## Explanation

The **processing unit** is typically the **Central Processing Unit (CPU)**. It is made of two parts:

- **Control unit**: The **manager**. It fetches instructions, works out what they mean, and tells the other parts what to do and when.
- **Arithmetic Logic Unit (ALU)**: The **calculator and decision-maker**. It does **arithmetic** (math such as adding and subtracting) and **logic** (comparing values, such as "is this number bigger?").

**CPU = Control Unit + ALU**

The CPU is responsible for **interpreting and executing** instructions. It does this once the input interface has delivered the data to the system.

[insert image about the CPU made of the control unit and the ALU, connected to memory and input/output]

## Worked Example

**Task:** A program asks: "Is the typed number bigger than 10?" You type 14.

| Step | Part | What happens |
|------|------|--------------|
| 1 | Control unit | Reads the instruction and sends the numbers 14 and 10 to the ALU |
| 2 | ALU | Performs a **logic operation**: is 14 > 10? The answer is **True** |
| 3 | Control unit | Uses the result to decide the next step |

## Activity

Which part (control unit or ALU) does each job?

a. Adding 8 + 5
b. Telling the memory to send the next instruction
c. Checking if two numbers are equal

<details>
<summary><b>Answer</b></summary>

a. **ALU**
b. **Control unit**
c. **ALU**

</details>

---

# 1.4 Components (2): Memory, Input, and Output

## Explanation

### Input Controllers

An **input controller** is made of **circuitry** (electronic circuits) and other components. It **receives input signals** from the input devices, **processes the data**, and **sends it** to the CPU. A **signal** is a pattern of electricity that carries information. You can think of the controller as a **translator** between the device and the CPU.

[insert image about an Input/Output controller device]

### Input Devices

**Input devices** are the tools that users interact with to give data to the computer. Each one is built to handle a specific kind of data:

| Device | What it does |
|--------|--------------|
| **Keyboard** | Captures typed text |
| **Mouse** | Detects movements and clicks and turns them into **cursor** movements (the cursor is the pointer on the screen) |
| **Touchscreen** | Combines input and output by detecting touches right on the display |
| **Scanner** | **Digitizes** physical documents, which means it turns paper into computer-readable data |
| **Microphone** | Captures sound |

### Input Data

**Input data** is the actual information or signals sent to the computer for processing. Its form depends on the input device:

| Type | Example device |
|------|----------------|
| **Text** | Keyboard |
| **Audio** | Microphone |
| **Images or video** | Camera |
| **Sensor signals** (temperature, light, or motion) | **Sensors** (devices that measure something in the real world) |

Input data can also include **commands**, **raw numbers**, and **touch gestures** (such as swiping or pinching). The **quality** and **type** of input data decide how the system handles it. For example, a blurry photo or noisy audio is harder for the computer to use than a clear one.

### Memory and Output

After processing, the CPU **communicates** with **memory** (to keep programs and data), **storage**, and **output devices** (to show the result). **Output** is the result the computer gives back to the user, such as a display or a printout.

[insert image about an input example: keyboard to computer, and an output example: computer to printer]

## Worked Example

**Task:** Match the input device and the kind of input data for each case.

| Situation | Input device | Input data |
|-----------|--------------|------------|
| Typing an email | Keyboard | Text |
| Recording a voice note | Microphone | Audio |
| Taking a photo | Camera | Images |
| A thermometer chip reading 22°C | Sensor | Sensor signal |
| Swiping across a phone screen | Touchscreen | Touch gesture |

## Activity

a. What does an input controller do?
b. Which input device turns a paper document into computer data?
c. Name the input data type for each: (i) a song recorded by a microphone, (ii) a motion reading from a sensor.
d. Give two examples of input data that are not text, audio, images, or sensor signals.

<details>
<summary><b>Answer</b></summary>

a. It **receives signals from the input device, prepares the data, and passes it to the CPU**.
b. A **scanner**.
c. (i) **Audio** (ii) **Sensor signal**
d. For example: **commands**, **raw numbers**, or **touch gestures**.

</details>

---

## Stage 1 Summary

- The **von Neumann model** has four subsystems: **Memory**, **ALU**, **Control Unit**, and **Input/Output**.
- An **input system** has an **input interface**, **input controllers**, **input devices**, and **input data**.
- **Input controllers** receive signals from devices, prepare the data, and pass it to the CPU.
- **Input devices** (keyboard, mouse, touchscreen, scanner, microphone) each handle specific kinds of data.
- **Input data** can be text, audio, images or video, sensor signals, commands, raw numbers, or touch gestures.
- The **processing unit** (usually the **CPU**) **analyzes** data (converts it to binary), **executes** the operations, and **communicates** with memory, storage, and output devices.
- The **CPU** is made of the **control unit** (manager) and the **ALU** (arithmetic and logic).

# Stage 1: Von Neumann Model (Output and Storage)

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions.
2. Describe where output and storage fit in the von Neumann model.
3. Explain how a result travels from the CPU to an output device or to storage.
4. Describe the three parts of an output system: the output interface, output devices, and digital-to-analog conversion.
5. Explain the difference between primary and secondary storage.

**Topics covered:**

- Definition
- Process (fetch-decode-execute)
- Components (1): CPU (control unit and ALU)
- Components (2): Memory, Input, and Output

---

# 1.1 Definition

## Explanation

The **von Neumann model** describes a computer as four **subsystems** (smaller parts that each do one main job):

| Subsystem | Its job |
|-----------|---------|
| **Memory** | Stores both programs and data |
| **Arithmetic Logic Unit (ALU)** | Performs calculations and logic operations |
| **Control Unit** | Manages all operations |
| **Input/Output** | Moves data between the computer and the outside world |

In this stage, we focus on what happens **after** the computer has worked on the data:

- **Output** is the data or information that a computer **sends to an external device or to the user** after it has processed the input. (An **external device** is a device outside the computer's main body, such as a printer.)
- **Storage** is the part of the computer that **saves and keeps data**. It holds both **programs** (lists of instructions) and **data** (the information those programs use or create). The von Neumann model describes storage in exactly this way: it holds **both the program instructions and the data the program works on**.

In modern computers, all stored data is in **binary** form, which means it is written with only `0` and `1`. These binary patterns can stand for anything: text, images, or videos.

The basic workflow of a computer looks like this:

**Input → Process → Output**, with **Storage** connected to the Process step (data can be saved there and brought back).

[insert image about the Input -> Process -> Output flow with Storage underneath Process]

## Worked Example

**Task:** You type a sentence in a document, then print it and save it.

| What happens | Subsystem / function |
|--------------|----------------------|
| You type the sentence | Input |
| The computer works with the text | Process (CPU) |
| The page comes out of the printer | Output |
| The document is saved for later | Storage |

## Activity

Is each example **output** or **storage**?

a. A photo is shown on a monitor.
b. A file is kept on a hard drive so you can open it tomorrow.
c. A song is played through speakers.

<details>
<summary><b>Answer</b></summary>

a. **Output**
b. **Storage**
c. **Output**

</details>

---

# 1.2 Process (Fetch-Decode-Execute)

## Explanation

The computer follows its program **one instruction at a time**. For each instruction, it repeats the **fetch-decode-execute cycle**:

1. **Fetch**: The control unit gets the next instruction from memory.
2. **Decode**: The control unit works out what the instruction means.
3. **Execute**: The instruction is carried out.

Output and storage are often the final results of this cycle. Here is **how the process works**:

1. The CPU finishes **processing** the input data.
2. The CPU sends the results to the **correct output subsystem**.
3. The output data travels to the **connected device** (such as a monitor or printer).
4. The device **displays**, **prints**, or **plays** the result. The **format** of the output depends on the type of data and on the output device being used.

At the same time, the results (and the program itself) can be **saved** in storage so the computer can use them again later.

[insert image about the fetch-decode-execute cycle ending with a result sent to an output device or to storage]

## Worked Example

**Task:** A program has two instructions: (1) "Add 4 and 6", (2) "Show the result on the screen."

| Cycle | Step | What happens |
|-------|------|--------------|
| 1 | Fetch | The control unit gets "Add 4 and 6" from memory |
| 1 | Decode | It works out that this means "add" and tells the ALU |
| 1 | Execute | The ALU calculates 10, and the result is stored in memory |
| 2 | Fetch | The control unit gets "Show the result on the screen" |
| 2 | Decode | It works out that the result must go to the output subsystem |
| 2 | Execute | The CPU sends 10 to the monitor, which **displays** it |

## Activity

a. Put these in the correct order: **The monitor displays the result**, **The CPU processes the data**, **The CPU sends the result to the output subsystem**.
b. What decides the format of the output?

<details>
<summary><b>Answer</b></summary>

a. **The CPU processes the data → The CPU sends the result to the output subsystem → The monitor displays the result**
b. The **type of data** and the **output device** being used.

</details>

---

# 1.3 Components (1): CPU (Control Unit and ALU)

## Explanation

The **Central Processing Unit (CPU)** is the "brain" of the computer. It is made of two parts:

- **Control unit**: The manager. It directs where data goes, including sending results to the right output device or to storage.
- **Arithmetic Logic Unit (ALU)**: Does the calculations and comparisons that **produce the results**.

**CPU = Control Unit + ALU**

The CPU works with **digital signals**, which are signals made of `0`s and `1`s. This matters for output, because some devices need a different kind of signal. For example, speakers need **analog signals** (smooth, continuously changing waves). So the computer needs a special step to convert one into the other. We look at this in the next section.

[insert image about the CPU sending results to output devices and to storage]

## Worked Example

**Task:** The ALU calculates a total of 25. Show how the control unit handles it.

| Step | Part | What happens |
|------|------|--------------|
| 1 | ALU | Calculates the result: 25 |
| 2 | Control unit | Sends 25 to the **output subsystem** so the monitor can show it |
| 3 | Control unit | Also sends 25 to **memory** so it is kept for later steps |

## Activity

Which part of the CPU does each job?

a. Calculating 12 + 13
b. Deciding that the result should go to the printer
c. Comparing two numbers to see which is bigger

<details>
<summary><b>Answer</b></summary>

a. **ALU**
b. **Control unit**
c. **ALU**

</details>

---

# 1.4 Components (2): Memory, Input, and Output

## Output

### Explanation

The **output system** is generally made of **three parts**:

**1. Output interface**

This part sends processed data from inside the computer **out to the world**, to a user or to another device. It has two sides:

- **Hardware**: The output devices.
- **Software**: **Drivers**, which are small programs that manage the communication between the computer and a device.

**2. Output devices**

These devices take processed data and **present it in a form people can use**:

| Device | What it does |
|--------|--------------|
| **Monitor (display)** | Converts digital data into visual information: text, images, or video |
| **Printer** | Produces a **hard copy**, which is a paper copy of documents or images |
| **Speakers** | Output **audio signals** after the computer has processed the sound data |

**3. Digital-to-analog conversion**

Computers use **digital signals**. But some devices, like speakers, need **analog signals**. A **sound card** inside the computer converts digital audio files into **analog waves** that speakers can play. The part that does this job is the **Digital-to-Analog Converter (DAC)**.

A DAC works in these steps:

| Step | Part | What it does |
|------|------|--------------|
| 1 | **Digital input** | The digital number comes in |
| 2 | **n-bit DAC register** | Holds the digital input (*n-bit* means a number made of n bits) |
| 3 | **Voltage switching** | Each bit switches a **reference voltage** (a steady, known voltage) on or off |
| 4 | **Resistive summing circuit** | Adds the switched voltages together into one voltage |
| 5 | **Output amplifier** | Makes the signal stronger |
| 6 | **Analog output** | The smooth analog signal goes out to the device |

[insert image about a digital-to-analog converter flowchart from digital input to analog output]

### Worked Example

**Task (simplified):** A 4-bit DAC receives the digital number `1010`. Each step of value equals 0.5 volts.

1. Convert `1010` to decimal: 8 + 2 = **10**
2. Voltage = 10 × 0.5 V = **5 volts**

So the digital number `1010` becomes an analog voltage of **5 V**. A different number would give a different voltage, and a stream of many numbers per second forms a smooth sound wave.

**Task (device choice):**

| Result wanted | Device | Needs digital-to-analog conversion? |
|---------------|--------|-------------------------------------|
| Read a web page | Monitor | No |
| Get a paper copy of a form | Printer | No |
| Hear a song | Speakers | **Yes** |

### Activity

a. What does a driver do?
b. A 4-bit DAC receives `0110`, with 0.5 volts per step. What voltage does it output?
c. Why do speakers need a sound card?

<details>
<summary><b>Answer</b></summary>

a. A **driver** is software that manages the communication between the computer and a device.
b. `0110` = 4 + 2 = 6, and 6 × 0.5 V = **3 volts**.
c. Speakers need **analog** signals, but the computer's audio is **digital**. The sound card converts digital audio into analog waves.

</details>

---

## Memory and Storage

### Explanation

In the von Neumann model, **memory** keeps programs and data. In everyday computer terms, we call this **storage**. Storage keeps information for both **short** and **long** periods, and it comes in two kinds:

| Kind | Time scale | Example | When the power goes off |
|------|------------|---------|-------------------------|
| **Primary storage** | Short term | **RAM** (Random Access Memory), the fast working memory | Contents are usually **lost** (it is **volatile**) |
| **Secondary storage** | Long term | Hard drive (HDD), solid-state drive (SSD) | Contents are **kept** (it is **non-volatile**) |

Storage holds:

- **Programs**: The instructions the computer follows.
- **Data**: The information the programs use or create while they run.

Because all stored data is **binary**, the same patterns of 0s and 1s can stand for text, images, or videos.

[insert image about primary storage (RAM) and secondary storage (a drive) connected to the CPU]

### Worked Example

**Task:** You make a drawing and save it.

| Step | Where is the drawing? |
|------|-----------------------|
| 1 | While you draw, it is held in **primary storage (RAM)** so the CPU can use it quickly |
| 2 | You click **Save**, and it is copied to **secondary storage** (for example, an SSD) |
| 3 | You switch off the computer. RAM is cleared, but the saved drawing stays on the SSD |

### Activity

a. Which kind of storage holds data and programs for a short time while the computer is working?
b. Which kind keeps your files after the computer is turned off?
c. Why can the same storage hold text, pictures, and videos?

<details>
<summary><b>Answer</b></summary>

a. **Primary storage** (RAM)
b. **Secondary storage**
c. All data is stored in **binary**, and binary patterns can stand for any kind of data.

</details>

---

## Input (Quick Link)

**Input** is the data or commands the computer receives from users or devices, such as typing on a keyboard. It is the starting point of the workflow: input comes in, the CPU processes it, and the results go out through **output** or into **storage**. Together, input and output let the user and the computer interact.

---

## Stage 1 Summary

- The **von Neumann model** has four subsystems: **Memory**, **ALU**, **Control Unit**, and **Input/Output**.
- **Output** is the data a computer sends to a user or device after processing. The output system has an **output interface** (hardware plus **drivers**), **output devices** (monitor, printer, speakers), and **digital-to-analog conversion**.
- A **DAC** turns digital numbers into an analog signal, so devices like speakers can play sound.
- When the CPU finishes processing (**fetch-decode-execute**), it sends results to the right output device, and the device displays, prints, or plays them.
- The **control unit** directs where results go, and the **ALU** produces them.
- **Storage** keeps both **programs and data**, in binary. **Primary storage** (RAM) is short term and volatile, and **secondary storage** (HDD/SSD) is long term.

# Stage 2: Computer Hardware

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions.
2. Define hardware and tell the difference between internal and external hardware.
3. Describe common input devices: mouse, keyboard, microphone, camera, and touchpad.
4. Describe common output devices: monitor, printer, and speaker.
5. Explain the role of the main internal parts: motherboard, CPU, RAM, ROM, graphics card, and power supply.
6. Describe ports and external storage such as USB drives and memory cards.

**Topics covered:**

- Hardware Definition
- Input Devices: Mouse, Keyboard, Microphone, Camera, Touchpad
- Output Devices: Monitor, Printer, Speaker
- Internal Hardware: Motherboard, CPU, RAM, RAM vs ROM, Graphics Card, Power Supply
- Ports and External Storage: USB, Memory Card

---

# 2.0 Hardware Definition

## Explanation

**Hardware** means the **physical parts of a computer**, the parts you can see and touch. The programs that run on the hardware are called **software**.

Hardware can be split into two groups:

| Group | Meaning | Examples |
|-------|---------|----------|
| **Internal hardware** | Parts **inside** the computer case | Motherboard, CPU, RAM, graphics card, power supply |
| **External hardware** | Parts **outside** the case that connect to the computer. These are also called **peripherals** | Keyboard, mouse, monitor, printer, speakers |

Hardware can also be sorted by its job:

- **Input devices** send data **into** the computer.
- **Output devices** show or deliver results **out of** the computer.
- **Internal hardware** processes, stores, and moves the data.
- **Ports and external storage** connect devices and keep data outside the main case.

[insert image about the main hardware of a computer: monitor, keyboard, mouse, and the case with internal parts]

## Worked Example

**Task:** Sort each item into **internal** or **external** hardware.

| Item | Group |
|------|-------|
| Keyboard | External |
| CPU | Internal |
| Printer | External |
| RAM | Internal |

## Activity

a. What is hardware?
b. Is a mouse internal or external hardware?
c. Is a word processor program hardware or software?

<details>
<summary><b>Answer</b></summary>

a. The **physical parts** of a computer that you can touch.
b. **External** (it is a peripheral that connects to the computer).
c. **Software** (it is a program, not a physical part).

</details>

---

# 2.1 Input Devices

## Explanation

**Input devices** are the devices used to **give data and commands to the computer**.

| Device | What it does |
|--------|--------------|
| **Keyboard** | One of the most common input devices. Each key matches a **character** (a letter, number, or symbol), a **function**, or a **command**. When you press a key, it creates a **signal** (a small pattern of electricity) that the computer understands as an action, such as typing a letter or running a shortcut. |
| **Mouse** | A **pointing device**: moving it moves a **cursor** (the pointer) on the screen. It lets you **click**, **select**, and **drag** objects in a **graphical user interface (GUI)**, which is a screen with windows, icons, and buttons. Modern mice often have extra buttons and a **scroll wheel**. |
| **Touchpad** | A flat, **touch-sensitive surface**, usually found on laptops. Moving your finger across it moves the cursor, and tapping works like a click. Many touchpads also understand **gestures** (finger movements such as two-finger scrolling). |
| **Camera** | A **visual** input device that **captures images or video** and sends the data to the computer. |
| **Microphone** | Turns **sound waves into electric signals**, so audio can enter the computer. |

**Types of cameras:**

- **Webcam**: A built-in or external camera on a computer, used for video calls.
- **Mobile camera**: Built into a smartphone or tablet. It has a **lens**, a **sensor** (which detects light), and an **image processor**, like a standalone camera but smaller.
- **Digital camera**: Higher quality, often used for photography and video production.

**Types of microphones:**

- **Condenser**: Very sensitive, often used in studios.
- **Dynamic**: Durable, often used for live sound.
- **USB microphone**: **Plug-and-play** (ready to use as soon as you connect it) and good for everyday use.

[insert image about a keyboard, a mouse, a touchpad, a webcam, and a microphone]

## Worked Example

**Task:** You join a video call and type a message in the chat. Name the input devices used.

| What you do | Input device |
|-------------|--------------|
| Show your face | Webcam (camera) |
| Speak | Microphone |
| Type the chat message | Keyboard |
| Move the pointer to the "Send" button on a laptop | Touchpad (or mouse) |

## Activity

Name the input device for each job:

a. Recording the sound of a live concert in a tough, durable way.
b. Moving the cursor on a laptop by sliding your finger.
c. Capturing a photo with your phone.
d. Pressing `Ctrl + C` to copy text.

<details>
<summary><b>Answer</b></summary>

a. **Dynamic microphone**
b. **Touchpad**
c. **Mobile camera**
d. **Keyboard**

</details>

---

# 2.2 Output Devices

## Explanation

**Output devices** present the **results of processed data** to the user. After the computer has processed the input, output devices share the results in different forms: **visual** (to see), **auditory** (to hear), or **physical** (to hold).

| Device | What it does |
|--------|--------------|
| **Monitor** | Also called a **display screen**. It shows data as graphics, text, or video. |
| **Printer** | Turns digital data into a **physical form** by printing on paper. |
| **Speaker** | Turns digital data into **sound**. |

### Monitor

Monitors come in several types: **LCD**, **LED**, and **OLED**. They also differ in two measurements:

- **Resolution**: The number of tiny dots (**pixels**) that make up the picture. More pixels give a clearer picture.
- **Refresh rate**: How many times per second the screen **updates** the picture, measured in **hertz (Hz)**. A higher rate makes motion look smoother.

Monitors display the **desktop**, applications, and media, and they give feedback on what the user does. **High-definition** displays are important for graphic design, gaming, and video production, where accurate visuals matter.

### Printer

Printers produce **hard copies** (paper copies) of documents. Common types:

- **Inkjet** and **laser** printers: Used for standard documents and photos.
- **3D printers**: Build **objects layer by layer** from a digital model. They are used in manufacturing, engineering, and medicine.

### Speaker

Speakers **convert digital data into sound**, such as music, videos, alerts, and system notifications. They are important for multimedia and for **accessibility**, because they let visually impaired users get information through sound.

[insert image about a monitor, an inkjet printer, a 3D printer, and speakers]

## Worked Example

**Task:** Choose the best output device.

| Need | Device | Why |
|------|--------|-----|
| Watch a movie | Monitor | Shows video |
| Get a paper copy of a school form | Printer (inkjet or laser) | Makes a hard copy |
| Make a physical model of a part from a digital design | 3D printer | Builds objects layer by layer |
| Hear a warning sound from the computer | Speaker | Produces audio |

**Refresh rate example:** A monitor with a refresh rate of 60 Hz updates the picture 60 times every second. A 144 Hz monitor updates it 144 times every second, so motion looks smoother.

## Activity

a. What is a pixel?
b. How many times per second does a 120 Hz monitor update the picture?
c. Which output device helps a visually impaired user hear information from the computer?
d. What is a hard copy?

<details>
<summary><b>Answer</b></summary>

a. One of the **tiny dots** that make up the picture on a screen.
b. **120 times** per second.
c. **Speaker**
d. A **paper copy** of a digital document or image.

</details>

---

# 2.3 Internal Hardware

## Motherboard

### Explanation

The **motherboard** is the **main circuit board** of the computer. It is the **backbone**: it connects all the essential parts and lets them **communicate**, including the CPU, memory, storage, and input/output devices.

The motherboard has several important features:

| Feature | What it does |
|---------|--------------|
| **CPU socket** | The physical spot where the CPU is installed |
| **Memory slots** | Slots where RAM modules are plugged in |
| **Expansion slots** | Slots (such as **PCIe**) for adding extra cards, like a graphics card |
| **Chipset** | A group of chips that controls how the CPU, memory, and other devices work together |
| **Data bus** | The wires that carry data between the parts |
| **Ports** | Connectors for devices (see 2.4) |

[insert image about a motherboard with the CPU socket, memory slots, expansion slots, and ports labeled]

### The Data Bus

A **data bus** is a set of wires that moves data between the CPU, memory, and other parts. Its **width**, measured in **bits**, decides how much data can be sent **at the same time**. A wider bus can carry more data in one go. Some important buses are:

| Bus | What it connects |
|-----|------------------|
| **Front-Side Bus (FSB)** | The CPU and main memory (found in older designs) |
| **PCIe (Peripheral Component Interconnect Express)** | High-speed parts such as graphics cards and SSDs |
| **SATA** | The motherboard and storage devices |
| **USB buses** | External devices such as keyboards and drives |

The **bus specs** (specifications, or technical details) decide the **data transfer rate** and the system's performance.

### The Chipset

The **chipset** acts as a controller for the CPU, memory, and other devices. In many computers, it is split into two parts:

- **Northbridge**: Connects the CPU to **high-speed** parts such as RAM and graphics cards.
- **Southbridge**: Manages **lower-speed** parts such as hard drives, USB ports, and expansion slots.

*(In many modern computers, the northbridge's work is built into the CPU itself, and a single chip handles the rest. The idea of fast and slow connections stays the same.)*

[insert image about motherboard architecture: CPU, northbridge, southbridge, memory bus, and PCI bus]

### Worked Example

**Task:** Compare data buses of different widths. How many transfers does it take to send 64 bits?

| Bus width | Bits moved per transfer | Transfers needed for 64 bits |
|-----------|------------------------|-------------------------------|
| 8 bits | 8 | 64 ÷ 8 = **8 transfers** |
| 32 bits | 32 | 64 ÷ 32 = **2 transfers** |
| 64 bits | 64 | 64 ÷ 64 = **1 transfer** |

A wider bus moves the same data in fewer steps.

### Activity

a. What is the motherboard's main job?
b. A 32-bit bus needs to send 128 bits. How many transfers are needed?
c. Which part of the chipset connects the CPU to RAM and graphics cards?

<details>
<summary><b>Answer</b></summary>

a. To **connect all the parts** of the computer and let them communicate.
b. 128 ÷ 32 = **4 transfers**
c. The **northbridge**

</details>

---

## CPU

### Explanation

The **Central Processing Unit (CPU)** is the **"brain"** of the computer. It **executes instructions** and **processes data**. It is installed in the **CPU socket** on the motherboard.

When the computer is switched on, the CPU starts the **boot sequence**. To **boot** means to start up. In the boot sequence, the CPU:

1. **Initializes** (sets up and checks) the hardware parts.
2. **Loads the operating system** (the main software that manages the computer) from storage into memory.

The CPU uses the data bus to **read and write data** to and from RAM and storage devices, which lets it work quickly.

[insert image about a CPU installed in a motherboard socket]

### Worked Example

**Task:** Put the start-up steps of a computer in order.

1. You press the power button.
2. The CPU starts the boot sequence.
3. The hardware parts are initialized.
4. The operating system is loaded from storage into memory.
5. The computer is ready to use.

### Activity

a. Where is the CPU installed?
b. What does "boot" mean?

<details>
<summary><b>Answer</b></summary>

a. In the **CPU socket** on the motherboard.
b. To **start up** the computer, setting up the hardware and loading the operating system.

</details>

---

## RAM and ROM

### Explanation

**RAM (Random Access Memory)** is the computer's fast, **temporary** working memory. When the CPU processes data, it keeps that data in RAM so it can reach it quickly. RAM is plugged into the **memory slots** on the motherboard. How much RAM there is, and how fast it is, affects the system's performance, especially for tasks that need fast access to data.

**ROM (Read Only Memory)** holds data that **cannot be easily changed**. It usually stores **firmware**, which is software built into the hardware to tell it how to start and work. For example, the **BIOS** is firmware that starts up a computer's hardware.

| Feature | RAM | ROM |
|---------|-----|-----|
| Full name | Random Access Memory | Read Only Memory |
| Purpose | Holds data and programs **in use right now** | Holds **start-up instructions** (firmware) |
| Can it be changed easily? | **Yes**, constantly | **No**, not easily |
| When the power goes off | Contents are **lost** (volatile) | Contents are **kept** (non-volatile) |
| Speed | Very fast | Slower than RAM |

[insert image about RAM modules in memory slots and a ROM chip holding firmware]

### Worked Example

**Task:** Decide whether RAM or ROM is used.

| Situation | Memory | Why |
|-----------|--------|-----|
| A browser with 10 open tabs | RAM | It needs fast, changeable memory |
| The instructions a computer uses to start up | ROM | They must stay when the power is off |
| A game being played | RAM | The CPU needs the data quickly |

### Activity

a. Which memory is lost when the computer is switched off?
b. What is firmware?
c. Which memory is better for holding the start-up instructions, RAM or ROM?

<details>
<summary><b>Answer</b></summary>

a. **RAM**
b. **Software built into hardware** that tells the hardware how to start and work.
c. **ROM**

</details>

---

## Graphics Card

### Explanation

A **graphics card** is an **expansion card** that handles **images and video**. It has its own processor, called a **GPU (Graphics Processing Unit)**, which is built to draw pictures very quickly. It plugs into a **PCIe expansion slot** on the motherboard and sends the picture to the monitor.

A **graphics card** is important for gaming, video editing, and graphic design. Other **expansion cards** work the same way:

- **Sound card**: Improves audio for tasks like professional audio work.
- **Network card**: Connects the computer to a network.

Each expansion card has its own resources and **communicates with the CPU through the motherboard**. This lets users **customize** their computers for the performance they need.

[insert image about a graphics card plugged into a PCIe expansion slot]

### Worked Example

**Task:** A designer edits 4K video. Which hardware helps most?

| Part | Why it helps |
|------|--------------|
| Graphics card (GPU) | Draws images and video quickly |
| RAM | Holds the video data being edited |
| CPU | Runs the editing program |

### Activity

a. What does GPU stand for?
b. Which slot is a graphics card plugged into?
c. Name another type of expansion card.

<details>
<summary><b>Answer</b></summary>

a. **Graphics Processing Unit**
b. A **PCIe expansion slot** on the motherboard
c. A **sound card** (or **network card**)

</details>

---

## Power Supply

### Explanation

The **power supply unit (PSU)** gives the computer the **electricity** it needs. The electricity from a wall outlet is **AC (alternating current)**, but computer parts need **DC (direct current)** at **lower voltages**. The PSU:

- **Converts** AC from the wall into low-voltage DC.
- **Sends power** through cables to the motherboard, drives, and other parts.

A PSU is rated in **watts (W)**. A more powerful computer, such as one with a strong graphics card, needs a PSU with a higher watt rating.

[insert image about a power supply unit with its cables going to the motherboard and drives]

### Worked Example

**Task:** A computer's parts need about 350 W in total. Which PSU is suitable?

| PSU | Suitable? | Why |
|-----|-----------|-----|
| 250 W | No | Not enough power |
| 500 W | Yes | Covers 350 W with room to spare |

### Activity

a. What does a power supply unit convert?
b. If you add a powerful graphics card, why might you need a bigger PSU?

<details>
<summary><b>Answer</b></summary>

a. **AC** electricity from the wall into low-voltage **DC** for the computer's parts.
b. A powerful graphics card uses **more electricity**, so the PSU must be able to supply more watts.

</details>

---

# 2.4 Ports and External Storage

## Explanation

**Input/output ports** are the **physical connectors** on a computer, such as **USB ports**, **audio jacks**, and **HDMI ports**. They let you connect devices to the computer. There are two types:

| Type | What it connects | Examples |
|------|------------------|----------|
| **Internal port** | The motherboard to devices **inside** the case | Hard disk, CD drive, internal Bluetooth |
| **External port** | The motherboard to devices **outside** the case | Mouse, printer, USB drive |

[insert image about different port types: USB-A, USB-C, HDMI, audio jack, ethernet, DisplayPort]

### USB (Universal Serial Bus)

A **USB port** can connect many kinds of external devices: external hard disks, printers, scanners, mice, keyboards, and more. USB comes in different **shapes** (such as Type A, Type B, and Type C) and different **versions**, which have different **speeds**. Speed is measured in **megabits per second (Mbps)**, where one **megabit** is one million bits.

| USB version | Maximum speed |
|-------------|---------------|
| USB 1.1 (an early version) | 12 Mbps |
| USB 2.0 | 480 Mbps |
| USB 3.0 | 5,000 Mbps (5 Gbps) |

A **USB flash drive** is a small, portable storage device that plugs into a USB port. It is plug-and-play and often used to move files between computers.

### Memory Card

A **memory card** is a small, thin **flash storage** card used to store data in cameras, phones, and other devices. A common type is the **SD card** (Secure Digital card), and a smaller version is the **microSD card**. You can read a memory card by putting it in a **card slot** or in a **card reader** (a small device that plugs into a USB port).

**External storage** means any storage that is not built permanently inside the computer, such as USB flash drives, external hard drives, and memory cards. It is useful for backups and for carrying files from one device to another.

[insert image about a USB flash drive and an SD memory card]

## Worked Example

**Task:** How long does it take to copy a 600 MB file over each USB version? (A **byte** is 8 bits, so 1 megabyte (MB) = 8 megabits (Mb). These are the best-case speeds. Real speeds are usually a little lower.)

1. Convert the file size: 600 MB × 8 = **4,800 megabits**
2. Time at 12 Mbps (USB 1.1): 4,800 ÷ 12 = **400 seconds** (about 6.7 minutes)
3. Time at 480 Mbps (USB 2.0): 4,800 ÷ 480 = **10 seconds**

A newer USB version moves the same file much faster.

## Activity

a. Name two examples of external ports.
b. How long does it take to copy a 60 MB file at 480 Mbps? (Hint: 60 MB × 8 = 480 megabits.)
c. What device can you use to read an SD card if your computer has no card slot?
d. Give two examples of external storage.

<details>
<summary><b>Answer</b></summary>

a. For example, a **USB port** and an **HDMI port** (or an audio jack).
b. 480 ÷ 480 = **1 second**
c. A **card reader** that plugs into a USB port.
d. For example, a **USB flash drive** and a **memory card** (or an external hard drive).

</details>

---

## Stage 2 Summary

- **Hardware** is the physical part of a computer. **Internal hardware** is inside the case, and **external hardware** (peripherals) connects from outside.
- **Input devices** send data into the computer: **keyboard**, **mouse**, **touchpad**, **camera**, and **microphone**.
- **Output devices** present results: **monitor** (resolution and refresh rate), **printer** (inkjet, laser, 3D), and **speaker**.
- The **motherboard** connects all the parts through the **data bus**, the **chipset**, **memory slots**, **expansion slots**, and **ports**.
- The **CPU** is the brain. It starts the boot sequence and uses the data bus to work with RAM and storage.
- **RAM** is fast, temporary working memory, and **ROM** keeps firmware that starts the hardware.
- A **graphics card (GPU)** handles images and video, and the **power supply** converts wall AC into low-voltage DC for the computer.
- **Ports** connect devices. **USB** connects many kinds of devices, and **memory cards** and USB drives provide portable **external storage**.

# Stage 2: Computer Hardware (Motherboard Power and BIOS, CPU, and GPU)

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions.
2. Explain how the motherboard shares power and how the BIOS/UEFI starts the computer.
3. Describe the CPU and the fetch-decode-execute cycle.
4. Explain what decides a CPU's speed: clock speed, cache, bus speed, and threads.
5. Describe the GPU, how it works, and why it is useful for graphics, gaming, and AI.

**Topics covered (from Internal Hardware):**

- Motherboard (power distribution and BIOS/UEFI)
- CPU
- Graphics Card (GPU)

---

# 2.3 Internal Hardware

**Hardware** means the physical parts of a computer. **Internal hardware** means the parts that sit **inside** the computer case. The **motherboard** is the main circuit board that connects them all, so it is a good place to start.

---

## Motherboard: Power Distribution and BIOS/UEFI

### Explanation

#### Power distribution

The **power supply unit (PSU)** brings electricity into the computer. The **motherboard** then **shares (distributes) this power** with the other parts, including the **CPU**, **memory**, and **peripheral devices** (devices that connect to the computer, like a mouse or printer).

Each part needs a different amount of power. The motherboard has **voltage regulation circuits**. **Voltage** is the "push" of electricity, measured in **volts**. These circuits make sure **each part receives a steady, correct level of voltage**. This is very important for **reliability** (the computer keeps working without crashing) and for **performance**.

#### BIOS/UEFI

The motherboard also holds a special piece of **firmware**. **Firmware** is software stored permanently inside a hardware device to tell it how to work. This firmware is called:

- **BIOS (Basic Input/Output System)**: The older name.
- **UEFI (Unified Extensible Firmware Interface)**: The newer version that replaces BIOS in most computers.

The BIOS/UEFI has two main jobs:

1. **It starts up the hardware** during the **boot process**. (To **boot** means to start the computer.) It **initializes** the hardware, which means it sets up and checks each part.
2. **It gives you a low-level way to configure the system.** (**Low-level** means close to the hardware, before the normal operating system has even started.) It stores important **settings** for hardware parts, and lets you change the **boot order**, which is the order in which the computer looks for an operating system, and some **hardware performance options**.

[insert image about the motherboard sharing power from the PSU to the CPU, memory, and peripherals]

[insert image about a BIOS/UEFI settings screen showing boot order]

### Worked Example

**Task:** A computer has a USB drive plugged in, and you want to start it from the drive instead of the SSD.

| Step | What happens |
|------|--------------|
| 1 | You turn on the computer and open the BIOS/UEFI settings |
| 2 | You change the **boot order** so the USB drive is first and the SSD is second |
| 3 | You save and restart |
| 4 | The BIOS/UEFI initializes the hardware, then looks for an operating system on the USB drive first |

### Activity

a. What does the motherboard do with the electricity it receives from the PSU?
b. Why does the motherboard have voltage regulation circuits?
c. What do BIOS and UEFI stand for?
d. Name two things you can change in the BIOS/UEFI.

<details>
<summary><b>Answer</b></summary>

a. It **distributes** the power to the CPU, memory, and peripheral devices.
b. To make sure **each part gets a stable, correct power level**, which keeps the computer reliable and working well.
c. **Basic Input/Output System** and **Unified Extensible Firmware Interface**.
d. For example: the **boot order**, **hardware settings**, and **performance options**.

</details>

---

## Central Processing Unit (CPU)

### Explanation

The **Central Processing Unit (CPU)** is the **"brain"** of the computer. It **executes instructions** (carries out the steps of programs) and **processes data**. It sits in the **CPU socket** on the motherboard.

When the computer is switched on, the CPU begins the **boot sequence**: it **initializes the hardware** and **loads the operating system** from storage into memory.

Inside the CPU are **millions or even billions of transistors**. A **transistor** is a tiny electronic **switch** that is either on or off. This matches **binary** (the system of `0`s and `1`s), so the CPU receives all its data in binary.

#### The fetch-decode-execute cycle

After the CPU receives input, it follows three steps for every instruction:

| Step | What happens |
|------|--------------|
| **1. Fetch** | The CPU gets the instruction from **RAM**. It uses the **address bus** (a set of wires that carries a memory **address**, which is a location number) to find where the instruction is stored. The instruction is then loaded into the CPU. |
| **2. Decode** | The CPU works out **what the instruction means**, by breaking it into smaller parts it can carry out. |
| **3. Execute** | The CPU carries out the instruction using its **ALU**. The result is stored back in RAM or sent to an **output device**, as needed. |

This cycle repeats in a **continuous loop**, which lets the CPU do complicated tasks quickly.

[insert image about the fetch-decode-execute cycle between the CPU, main memory, and the I/O system]

#### Parts of the CPU

- **Control unit**: Directs how the processor works. It manages the flow of data between the CPU and other parts by **sending signals** that coordinate actions, such as reading from or writing to memory.
- **Arithmetic Logic Unit (ALU)**: The part that does the **actual computing**. It does **arithmetic operations** (add, subtract, multiply, divide) and **logic operations** (comparisons, and the operations AND, OR, and NOT). It takes its inputs from the CPU's **registers**, which are tiny, very fast storage spots inside the CPU, and then outputs the result.
- **Program counter**: A register that holds the **address of the next instruction** to fetch.
- **Instruction register (IR)**: A register that holds the **instruction currently being decoded or executed**.

[insert image about the inside of a CPU: program counter, registers, ALU, control unit, and IR]

#### What decides a CPU's speed?

| Factor | Meaning |
|--------|---------|
| **Clock speed** | How many **cycles** (basic steps) the CPU can perform per second. It is measured in **GHz** (gigahertz). 1 GHz = 1 billion cycles per second. A higher clock speed means faster processing. |
| **Cache (L1, L2, L3)** | Small, very fast memory **inside the CPU** that keeps frequently used data and instructions. **L1** is the fastest but smallest. **L3** is larger but slower. Cache saves time compared to fetching from RAM. |
| **Bus speed** | How fast data travels between the CPU and other parts, like RAM and peripheral devices. A **bus** is a communication path that lets data travel between parts. |
| **Threads** | A **thread** is the smallest unit of work that the operating system can schedule. Modern CPUs can handle **many threads at once**, which is called **multithreading**. |

CPUs improve over time mostly by raising clock speed and making cache work more efficiently.

#### Reading a real CPU's details

The program **CPU-Z** shows information about a computer's CPU. For a laptop with an **Intel Core i5-12500H**, it shows:

| Detail | Value | Meaning |
|--------|-------|---------|
| Package | Socket 1744 FCBGA | How the CPU is attached to the motherboard |
| Max TDP | 45 W | The most power (and heat) the CPU is designed to handle, in watts |
| Cores | 4 P-cores + 8 E-cores = 12 | A **core** is an independent processing unit inside the CPU. P-cores are built for power, and E-cores for saving energy. |
| Threads | 16 | How many threads it can handle at once |
| Level 3 cache | 18 MB | The shared L3 cache |
| Bus speed | about 99.76 MHz | The speed of the connection to other parts |
| Core speed | 1695.85 MHz at that moment | The current clock speed (it changes with the workload) |

[insert image about the CPU-Z program showing the specs of an Intel Core i5-12500H]

### Worked Example

**Task 1:** Follow one instruction through the cycle. The instruction "Add 4 and 6" is stored at memory address 100.

| Step | What happens |
|------|--------------|
| Fetch | The program counter points to address 100. The CPU uses the address bus to get the instruction from RAM. |
| Decode | The control unit works out that it means "add". |
| Execute | The ALU calculates 4 + 6 = 10. The result is stored back in RAM. |
| Next | The program counter moves to the next address, and the cycle repeats. |

**Task 2 (clock speed, simplified):** A CPU runs at 3 GHz, and each instruction takes 3 cycles.

1. 3 GHz = 3 billion cycles per second
2. Instructions per second = 3 billion ÷ 3 = **1 billion instructions per second**

### Activity

a. Put these steps in order: **Execute**, **Fetch**, **Decode**.
b. What is the ALU's job?
c. A CPU runs at 4 GHz. How many cycles does it perform each second?
d. Which cache is the fastest: L1, L2, or L3?
e. In the CPU-Z example, how many threads can the Intel Core i5-12500H handle?

<details>
<summary><b>Answer</b></summary>

a. **Fetch → Decode → Execute**
b. To do the **arithmetic** (math) and **logic** (comparison) operations.
c. 4 GHz = **4 billion** cycles per second.
d. **L1**
e. **16 threads**

</details>

---

## Graphics Processing Unit (GPU)

### Explanation

A **Graphics Processing Unit (GPU)** is a **specialized processor** made to handle complex calculations, mainly those used to **draw (render) visuals**, **run games**, and do tasks that need **parallel processing**, such as AI. (**Rendering** means turning data into a finished picture. **Parallel processing** means doing many tasks **at the same time**.)

The GPU works **alongside the CPU**, but it is built to perform **many repetitive calculations at once**. That makes it perfect for graphics-heavy work.

| | CPU | GPU |
|---|-----|-----|
| Style | A few powerful cores that handle varied tasks one after another | Many small cores that handle many simple tasks at the same time |
| Best at | General tasks, running the operating system and programs | Graphics, video, games, and AI calculations |

#### Core components of a GPU

| Component | What it does |
|-----------|--------------|
| **Cores** | Small processing units that run tasks **in parallel**. More cores usually mean better performance for many tasks at once. |
| **Memory (VRAM)** | Video RAM. Stores data needed for drawing, such as **textures** (surface pictures on objects) and **frame buffers**. It lets the GPU work fast without always using the system's RAM. |
| **Memory interface** | Controls the flow of data between the VRAM and the GPU cores. It affects how fast the GPU can reach stored data. Common memory types are **GDDR** (Graphics Double Data Rate), such as **GDDR6** or **GDDR6X**, built for high-speed transfers. |
| **Shaders** | Specialized units that handle **lighting, color**, and other visual effects. |
| **Rasterizer** | Turns **3D objects into pixels** to show on a flat, 2D screen. (A **pixel** is one tiny dot of a picture.) |
| **Frame buffer** | Holds the **finished image** before it is sent to the display. |
| **Control logic** | Directs the cores and **schedules** (organizes) their tasks. |

[insert image about the main parts inside a GPU]

#### How a GPU works

1. **Input data**: The CPU sends the GPU data, such as textures, **vertices** (corner points of 3D shapes), and shaders.
2. **Parallel processing**: The GPU's many cores split the data into small tasks and work on them **at the same time**.
3. **Rendering**: The tasks include calculating images, textures, and animations.
4. **Output**: The finished data is sent to the **display**, producing images or video.

#### What GPUs are used for

- **Complex visuals and rendering**: GPUs draw 2D and 3D graphics, animations, and video. In video editing, **CAD** (Computer-Aided Design, used to design objects), and animation, the GPU handles shading, textures, and polygon creation much faster than a CPU.
- **Gaming**: Modern games need **high frame rates** (many images per second), realistic lighting, shadows, and physics. GPUs make smooth, lifelike visuals possible, including in **virtual reality (VR)**.
- **Artificial intelligence and machine learning**: AI training uses a huge number of **matrix multiplications** (repeated multiplying of grids of numbers), which a GPU can do in parallel. Companies such as NVIDIA build specialized GPUs for AI.

#### Integrated GPUs

Some GPUs are **integrated**, which means they are **built into the CPU** instead of being a separate graphics card. Integrated GPUs are:

- **Energy-efficient**, so they suit **battery-powered devices** such as laptops.
- **Cost-effective**, because there is no need to buy a separate graphics card.

A **dedicated** GPU is a separate graphics card with its own VRAM. It is more powerful but costs more and uses more power.

#### What decides a GPU's speed?

| Factor | Meaning |
|--------|---------|
| **Core clock** | The speed at which the GPU cores run, in **MHz** (megahertz). It directly affects processing power. |
| **Memory clock** | The speed of the VRAM, in MHz. It shows how fast data can move between the memory and the GPU. |

[insert image about a CPU sending data to a GPU, which sends the final image to a display]

### Worked Example

**Task 1 (pixels per second):** A monitor shows 1920 × 1080 pixels at 60 frames per second. How many pixel updates does the GPU handle every second?

1. Pixels per frame = 1920 × 1080 = **2,073,600**
2. Pixels per second = 2,073,600 × 60 = **124,416,000**

That is more than 124 million pixel updates every second, which is why a GPU's parallel cores are so helpful.

**Task 2 (parallel processing):** There are 100 tasks, and each takes 1 second.

| Number of cores | Time needed |
|-----------------|-------------|
| 1 core | 100 seconds |
| 10 cores | 10 seconds |
| 100 cores | 1 second |

More cores working in parallel finish the work faster.

### Activity

a. What does GPU stand for?
b. What is parallel processing?
c. How many pixels are on a 3840 × 2160 (4K) screen?
d. Name two parts inside a GPU and what each one does.
e. Why is an integrated GPU a good choice for a laptop?

<details>
<summary><b>Answer</b></summary>

a. **Graphics Processing Unit**
b. Doing **many tasks at the same time**.
c. 3840 × 2160 = **8,294,400 pixels**
d. For example: **VRAM** stores textures and frame buffers; the **rasterizer** turns 3D objects into pixels; the **frame buffer** holds the finished image.
e. It is **energy-efficient**, which helps battery life, and **cost-effective**, because no separate graphics card is needed.

</details>

---

## Stage 2 Summary

- The **motherboard** distributes power from the PSU to the CPU, memory, and peripherals, and uses **voltage regulation circuits** to keep each part's power steady.
- The **BIOS/UEFI** is firmware that **initializes the hardware** during boot and lets you change settings, such as the **boot order**.
- The **CPU** is the "brain". It is built from billions of **transistors** and repeats the **fetch-decode-execute** loop.
- The **control unit** directs the CPU's work, and the **ALU** does arithmetic and logic.
- CPU speed depends on **clock speed**, **cache** (L1, L2, L3), **bus speed**, and **threads**.
- The **GPU** is a specialized processor that uses **parallel processing** for graphics, gaming, and AI.
- A GPU's main parts are **cores, VRAM, a memory interface, shaders, a rasterizer, a frame buffer, and control logic**.
- GPU speed depends on the **core clock** and the **memory clock**. **Integrated GPUs** are energy-efficient and low in cost, while **dedicated** GPUs are more powerful.

# Stage 2: Computer Hardware (Graphics Memory, RAM, ROM, and Storage)

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions.
2. Explain what VRAM is and read the main details of a graphics card.
3. Explain the difference between RAM and ROM, and where cache memory fits.
4. Describe what decides RAM performance: frequency, type, and timings.
5. Describe secondary storage devices (HDD, SSD, optical, USB flash drives, memory cards) and their strengths and weaknesses.
6. Explain how the CPU retrieves data using the fetch-decode-execute cycle and interrupts.

**Topics covered (from Internal Hardware and Ports and External Storage):**

- Graphics Card (VRAM)
- RAM
- RAM vs ROM
- USB and external storage (flash drives, memory cards)

---

# 2.3.2 Graphics Card: VRAM and Specs

## Explanation

A graphics card has its own fast memory called **VRAM** (Video RAM). It stores the data needed to draw pictures, such as textures and the final image before it is shown on screen.

VRAM comes in different **types**. Each new type is usually **faster at transferring data** than the one before it. For example, **GDDR6** is faster than **GDDR5**. (**GDDR** stands for Graphics Double Data Rate.) Newer types are common in modern graphics cards used for demanding jobs, such as gaming and video editing.

A **dedicated GPU** is a graphics card with its own VRAM. Here is a real example. A laptop with an **NVIDIA RTX 3050** graphics card shows these specs in the program **CPU-Z**:

| Detail | Value | What it means |
|--------|-------|---------------|
| Name | NVIDIA GeForce RTX 3050 Laptop GPU | The graphics chip's model |
| Code name | GA107 | The name of the chip's design |
| Technology | 8 nm | The size of the tiny parts inside the chip. A **nanometer (nm)** is one billionth of a meter. Smaller sizes usually mean more parts fit on the chip and it uses less power. |
| Max TDP | 80 W | The most power (and heat) the chip is designed to handle, in watts |
| GFX core clock | 210 MHz | The current speed of the GPU core (it changes depending on the workload) |
| Shader clock | 405 MHz | The current speed of the shaders, the units that handle lighting and color |
| Memory size | 4 GB | How much VRAM there is |
| Memory type | GDDR6 | The type of VRAM |
| Bus width | 128 bits | How many bits of data can move between the VRAM and the GPU at the same time |

[insert image about the CPU-Z program showing the specs of an NVIDIA GeForce RTX 3050 Laptop GPU]

## Worked Example

**Task:** The RTX 3050 has a **128-bit** memory bus. How many bytes can it move in one transfer, and how many transfers are needed to move 1,600 bytes?

1. 1 byte = 8 bits, so 128 bits ÷ 8 = **16 bytes per transfer**
2. 1,600 bytes ÷ 16 = **100 transfers**

A wider bus moves the same data in fewer transfers.

## Activity

a. What does VRAM store?
b. Which is the newer and faster memory type: GDDR5 or GDDR6?
c. How much VRAM does the RTX 3050 in the example have?
d. A memory bus is 256 bits wide. How many bytes can it move in one transfer?

<details>
<summary><b>Answer</b></summary>

a. Data needed for drawing images, such as **textures** and the **frame buffer**.
b. **GDDR6**
c. **4 GB**
d. 256 ÷ 8 = **32 bytes**

</details>

---

# 2.3.3 Storage

## Primary Storage: RAM, ROM, and Cache

### Explanation

**Storage** is the part of the computer that holds data the CPU and other components need to reach **right away** while the computer is working. There are two main groups: **primary storage** and **secondary storage**. We start with primary storage.

**RAM (Random Access Memory)** keeps data **temporarily** while the computer is running. RAM gives **very quick access** to data, but **everything in it is lost when the power goes off**. (This is called being **volatile**.) RAM acts as a **high-speed buffer**, which means a fast waiting area, between the CPU and slower storage devices such as hard drives. This lets the computer quickly reach the data it needs to run programs and carry out commands.

**ROM (Read Only Memory)** keeps data that **cannot be easily changed**. In modern computers, ROM usually holds **firmware**, which is software stored inside a hardware device to tell it how to work.

| Feature | RAM | ROM |
|---------|-----|-----|
| Full name | Random Access Memory | Read Only Memory |
| Holds | Programs and data in use right now | Firmware (start-up instructions) |
| Can it be changed easily? | Yes | No |
| When the power goes off | Contents are lost | Contents are kept |

[insert image about a RAM stick and a ROM chip, labeled RAM and ROM]

**Where RAM sits in the computer:**

- The **motherboard** has **memory slots** for **DRAM modules**. (**DRAM** is Dynamic RAM, the common type of RAM. A **module** is a small circuit board holding the memory chips.)
- Common module types are **DDR4** and **DDR5**. They have different speeds and sizes.
- How well the memory talks to the CPU also depends on the motherboard's **chipset** and **bus speed**.

**Cache memory:** In modern computers, the CPU usually has **cache memory**. It is a **smaller and faster** type of volatile memory **very close to the CPU**, and it keeps the most frequently used data so the CPU can reach it even faster than RAM.

### Worked Example

**Task:** Decide where each item is kept.

| Item | Where | Why |
|------|-------|-----|
| A game while you are playing it | RAM | Needs fast access, and is only needed while it runs |
| The instructions a computer uses to start up | ROM | They must stay when the power is off |
| The data the CPU uses again and again | Cache | Fastest access, right next to the CPU |

### Activity

a. Which memory loses its contents when the computer is switched off, RAM or ROM?
b. What does "buffer" mean when we say RAM is a high-speed buffer?
c. Name two RAM module types.
d. Where is cache memory located?

<details>
<summary><b>Answer</b></summary>

a. **RAM**
b. A **fast waiting area** between the CPU and slower storage, where data is held for quick access.
c. **DDR4** and **DDR5**
d. **Very close to the CPU** (inside or right next to it).

</details>

---

## RAM Performance

### Explanation

RAM performance is usually described using three things:

| Term | Meaning |
|------|---------|
| **RAM frequency** | How fast the RAM can **read and write** data, measured in **MHz** (megahertz, millions of cycles per second), for example 3200 MHz. A higher frequency means faster data transfer between the RAM and the CPU. |
| **RAM type** | The technology **generation**, such as DDR4 or DDR5. Newer types are usually faster and more efficient. |
| **RAM timings** | Numbers that show **latency**, which is the **delay** before data starts to arrive. **Lower numbers mean faster performance.** |

Here are the main details of a real RAM module, as shown in **CPU-Z**:

| Detail | Value | What it means |
|--------|-------|---------------|
| Type | DDR4 | The RAM generation |
| Size | 8 GB | The amount of memory |
| Channel | 1 × 64-bit | How data travels to the CPU: one path that is 64 bits wide |
| DRAM frequency | 1596.1 MHz | The speed of the RAM's clock |
| CAS latency (CL) | 22 clocks | The delay, counted in clock cycles, before data can be read. This is the best-known timing number. |
| RCD, RP, RAS, RC | 22, 22, 52, 74 clocks | Other timing numbers for opening and closing parts of the memory |
| Command rate | 1T | How quickly the memory accepts commands |

*(DDR memory sends data twice per clock cycle. That is why a clock of about 1600 MHz is sold as "3200" memory.)*

[insert image about the CPU-Z program showing the specs of a DDR4 RAM module]

### Worked Example

**Task:** Which RAM responds faster? Both modules run at 1596.1 MHz. Module A has CL = 22, and Module B has CL = 16.

1. One clock cycle lasts 1 ÷ 1596.1 million seconds, which is about **0.627 nanoseconds** (a **nanosecond** is one billionth of a second).
2. Module A: 22 × 0.627 ≈ **13.8 ns**
3. Module B: 16 × 0.627 ≈ **10.0 ns**

Module B has a **lower timing number**, so it has less delay and is **faster**.

### Activity

a. What does a lower timing number mean?
b. Which gives faster transfer: 2666 MHz or 3200 MHz RAM (same type)?
c. How much RAM is in the CPU-Z example?
d. Name the two RAM generations mentioned in this section.

<details>
<summary><b>Answer</b></summary>

a. **Less delay**, so faster performance.
b. **3200 MHz** (a higher frequency means faster transfer).
c. **8 GB**
d. **DDR4** and **DDR5**

</details>

---

## Secondary Storage and USB Drives

### Explanation

**Secondary storage** is **permanent** storage. It includes hard drives (HDD), solid-state drives (SSD), optical drives, and USB flash drives. Data **stays stored** here even when the computer is turned off.

| Device | How it works | Notes |
|--------|--------------|-------|
| **Hard Disk Drive (HDD)** | A traditional drive that stores large amounts of data on **spinning magnetic disks** called **platters** | Big capacity, slower, has moving parts |
| **Solid-State Drive (SSD)** | **Flash-based** storage (it uses electronic memory chips) with **no moving parts** | Much faster than an HDD |
| **Optical storage** | Discs such as **CDs, DVDs, and Blu-rays**, read by a laser | Used for media and backup copies |
| **USB flash drive** | A **portable, solid-state** storage device that plugs into a **USB port** | Used to move files between devices and for backups. Capacity ranges from a few gigabytes to several terabytes. |

A **memory card**, such as an **SD card**, is another small, portable flash storage device. It is commonly used in cameras and phones.

**Advantages of USB drives:**

- **Portability**: Small and light, so they are easy to carry.
- **Plug-and-play**: No installation is needed. You plug the drive into a USB port and it is ready to use.

**Disadvantages of USB drives:**

- **Limited lifespan**: Flash storage can only be written a limited number of times (called **write cycles**). For most people this does not matter unless the drive is used very heavily.
- **Easy to lose or damage**: Because they are so small, they can be misplaced or damaged if not handled carefully.

[insert image about different storage media: a floppy disk, USB drives, a CD, a hard drive, and an SD card]

### Worked Example

**Task:** Choose the best storage for each need.

| Need | Best choice | Why |
|------|-------------|-----|
| Carry a school project to another computer | USB flash drive | Portable and plug-and-play |
| Make a computer start and open programs quickly | SSD | Fast, with no moving parts |
| Store a large archive of old files cheaply | HDD | Large capacity |
| Keep the photos from a camera | Memory card (SD card) | Small, made for cameras |

### Activity

a. Which type of drive has spinning platters?
b. Give one advantage and one disadvantage of USB drives.
c. What is a write cycle?

<details>
<summary><b>Answer</b></summary>

a. The **HDD** (hard disk drive).
b. Advantage: for example, **portability** or **plug-and-play**. Disadvantage: for example, a **limited lifespan** or **easy to lose or damage**.
c. **One time data is written** to the flash storage. Flash storage can only handle a limited number of them.

</details>

---

## Data Access and Retrieval

### Explanation

Primary and secondary storage work together:

- **Primary storage (RAM)** is **much faster** than secondary storage, so the CPU can reach data quickly while it works. But because it is **volatile**, it needs a **constant power supply**. That is why data that is not in active use is **moved to secondary storage**.
- **Secondary storage** has **much more space** and keeps data for the long term, but it has **slower access**. It is used for saving documents, system files, applications, and **databases** (organized collections of data).

**How the CPU retrieves data: the fetch-decode-execute cycle**

| Step | What happens |
|------|--------------|
| **Fetch** | The CPU gets the instruction or data from memory |
| **Decode** | The CPU works out what action the instruction asks for |
| **Execute** | The CPU does the action, such as adding numbers or moving data |

**Input/Output (I/O) and interrupts**

I/O devices (like a keyboard or printer) send and receive data using **interrupts**. An **interrupt** is a **signal that pauses** the CPU's normal work so it can **handle an input or output task**. After that, the CPU **returns to the cycle** where it left off.

[insert image about the CPU pausing the fetch-decode-execute cycle to handle an interrupt from a keyboard]

### Worked Example

**Task:** You are running a program, and you press a key.

| Step | What happens |
|------|--------------|
| 1 | The CPU is in the middle of the fetch-decode-execute cycle for your program |
| 2 | The keyboard sends an **interrupt** signal |
| 3 | The CPU **pauses** the program and handles the key press (the input task) |
| 4 | The CPU **returns** to the cycle and carries on with the program |

### Activity

a. Why is data not in use moved from RAM to secondary storage?
b. Which has more storage space, primary or secondary storage?
c. What does an interrupt do?
d. Put in order: **Execute**, **Fetch**, **Decode**.

<details>
<summary><b>Answer</b></summary>

a. RAM is **volatile** and needs constant power, so data that must be kept is moved to **secondary storage**, which keeps it without power.
b. **Secondary storage**
c. It **pauses the CPU's normal processing** so it can handle an input or output task, then the CPU returns to the cycle.
d. **Fetch → Decode → Execute**

</details>

---

## Stage 2 Summary

- **VRAM** is the graphics card's own memory. Newer types (like **GDDR6**) are faster than older ones (like GDDR5). A **128-bit** bus moves 16 bytes per transfer.
- **RAM** is fast, temporary memory that loses its contents without power. **ROM** keeps **firmware** that cannot be easily changed. **Cache** is small, very fast memory near the CPU.
- **RAM performance** depends on **frequency** (MHz), **type** (DDR4 or DDR5), and **timings** (lower means less delay).
- **Secondary storage** keeps data without power: **HDD** (spinning platters), **SSD** (flash, no moving parts), **optical discs**, **USB flash drives**, and **memory cards**.
- **USB drives** are portable and plug-and-play, but they have a limited number of write cycles and are easy to lose or damage.
- **RAM** is faster and **secondary storage** is larger and permanent, so data not in use is moved to secondary storage.
- The CPU retrieves data using **fetch-decode-execute**. **Interrupts** pause that cycle so the CPU can handle input and output.

# Stage 3: Program Execution

## Learning Goals

By the end of this stage, you will be able to:

1. Identify core physical components of computers and explain basic functions.
2. Define program execution.
3. Name the main parts of the simple MARIE computer: the CPU, the ALU, and memory.
4. Explain what the registers (AC, PC, IR, MAR, MBR, InREG, OutREG) do.
5. Follow a program from memory through the fetch, decode, and execute steps.

**Topics covered:**

- Definition
- How Program Execution Works (from stored program to running task)

---

# 3.1 Definition

## Explanation

A **program** is a list of **instructions** that tells a computer what to do. **Program execution** is the process of the computer **carrying out those instructions, one after another**, until the task is finished. It begins when the program sits in memory, and it ends when the last instruction is done.

Real computers are very complicated. To understand program execution clearly, we use a **simple model computer** called **MARIE**. MARIE stands for **Machine Architecture that is Really Intuitive and Easy**. It shows the main ideas of how computers work without the extra complications of modern machines.

MARIE has **three core components**:

| Component | Its job |
|-----------|---------|
| **CPU (Central Processing Unit)** | The "brain". It executes the instructions of programs and manages the operations in the system. |
| **ALU (Arithmetic Logic Unit)** | The part of the CPU that does **arithmetic** (add, subtract, multiply, divide) and **logic** (compare, AND, OR, NOT). |
| **Memory** | Stores the **data** and the **program instructions**. |

[insert image about the MARIE architecture: the ALU and registers inside the CPU, connected to main memory]

### The CPU in MARIE

The CPU has three key parts:

- **Datapath**: A network of **registers**, the **ALU**, and **buses** that moves and processes data. A **bus** is a set of wires that carries information between parts.
- **Control Unit (CU)**: Directs the CPU's work. It **fetches** instructions from memory, **decodes** them (works out what they mean), and **sends signals** to the other parts so that they carry out the action.
- **Registers**: Very fast, small storage spots **inside the CPU** that hold data **temporarily** while the CPU works.

MARIE uses these registers:

| Register | Full name | What it holds |
|----------|-----------|---------------|
| **AC** | Accumulator | The data used in **arithmetic and logic** operations, and their results |
| **PC** | Program Counter | The **address of the next instruction** to run |
| **IR** | Instruction Register | The **instruction currently being executed** |
| **MAR** | Memory Address Register | The **address** of the data to be fetched or stored |
| **MBR** | Memory Buffer Register | The **data** being read from or written to memory (temporarily) |
| **InREG** | Input Register | Data **received from an input device**, such as a keyboard |
| **OutREG** | Output Register | Data **waiting to be sent to an output device**, such as a monitor |

### The ALU in MARIE

The ALU has these features:

- It usually has **multiple inputs** (the numbers it works on, called **operands**) and **one output** (the result).
- It may have a **status register** that records facts about the last operation, such as an **overflow** (the result was too big to fit) or a **zero** result. These can affect how the program continues.
- It **receives signals from the control unit** telling it which operation to do. Then it sends the result **back to a register**, often the **AC**.

### Memory in MARIE

- **Main memory (RAM)** is **volatile** (it loses its data when the power goes off). It is **random access**, which means any location can be reached directly without reading through the ones before it.
- MARIE's memory has **4K words**, and each **word** is **16 bits** long. (A **word** is the standard-sized chunk of data the computer handles at once. **4K** means 4 × 1,024 = **4,096** locations, with addresses from 0 to 4095.)
- Memory is a long series of **locations**, each with its own unique **address**. Memory can be **byte-addressable** (every byte has an address) or **word-addressable** (every word has an address). MARIE is **word-addressable**.
- Memory has two basic operations:
  - **Reading**: Copying data from a memory address into a register (such as the MBR).
  - **Writing**: Storing data from a register into a memory address.
- **Cache memory** is a smaller, faster memory close to the CPU. MARIE does not usually include it, but complex computers do.

The CPU and memory talk to each other through a **bus**, which carries three kinds of information: **addresses** (address lines), **data** (data lines), and **control signals** (control lines).

[insert image about the CPU connected to main memory by address lines, data lines, and control lines, with an I/O subsystem]

## Worked Example

**Task 1:** How many bits does MARIE's memory hold in total?

1. Number of words = 4,096
2. Bits per word = 16
3. Total bits = 4,096 × 16 = **65,536 bits**
4. In bytes: 65,536 ÷ 8 = **8,192 bytes** (8 KB)

**Task 2:** Match each job to the correct register.

| Job | Register |
|-----|----------|
| Holds the address of the next instruction | PC |
| Holds the result of an addition | AC |
| Holds data just read from memory | MBR |
| Holds the instruction being executed | IR |

## Activity

a. What is program execution?
b. What does MARIE stand for?
c. Which register holds the address of the data to be fetched or stored?
d. How many memory locations does MARIE have, and how many bits is each one?
e. Which register holds data coming from a keyboard?

<details>
<summary><b>Answer</b></summary>

a. The process of the computer **carrying out the instructions of a program**, one after another.
b. **Machine Architecture that is Really Intuitive and Easy**
c. The **MAR** (Memory Address Register)
d. **4,096** locations (4K), each **16 bits** long.
e. The **InREG** (Input Register)

</details>

---

# 3.2 How Program Execution Works

## From Stored Program to Running Task

### Explanation

Program execution follows a clear path. In MARIE, the full journey has these steps:

1. **Load** the program into memory.
2. **Fetch** an instruction from memory.
3. **Decode** the instruction.
4. **Execute** the instruction (this may involve memory, the ALU, or input/output).
5. **Repeat** steps 2 to 4 for the next instruction.
6. **Halt** (stop) when the program ends.

The CPU controls this cycle. The steps 2 to 4 are called the **fetch-decode-execute cycle**.

[insert image about the path of a program: loaded into memory, then fetch, decode, execute in a repeating loop, until halt]

### Worked Example

**Task:** Put these steps of running a program in order.

| Order | Step |
|-------|------|
| 1 | The program is loaded into memory |
| 2 | The CPU fetches the first instruction |
| 3 | The CPU decodes it |
| 4 | The CPU executes it |
| 5 | The CPU repeats the cycle for the next instruction |
| 6 | A Halt instruction ends the program |

### Activity

Which step comes first: fetching an instruction, or loading the program into memory?

<details>
<summary><b>Answer</b></summary>

**Loading the program into memory.** The CPU can only fetch an instruction that is already stored in memory.

</details>

---

## Step 1: Loading a Program into Memory

### Explanation

Memory stores **both the program's instructions and its data**. Every word in memory has a unique address.

To run a program, it is **loaded into memory** starting at a set address. In our examples, the program starts at **address 100**. (Memory addresses in MARIE are usually written in **hexadecimal**, the base-16 number system. So 100 means 100 in hexadecimal, which is 256 in decimal.)

Each instruction is a **16-bit binary number**, so it fits exactly in one word of memory.

In the diagram of the system, the memory holds the **program** and the **data**. Each memory location has an **address** (which says where it is) and **contents** (the 16 bits stored there).

[insert image about memory holding a program and data, each location with an address and 16-bit contents, connected to the CPU, keyboard, and monitor]

### Worked Example

**Task:** Show how this program and its data are laid out in memory. (Addresses are in hexadecimal. The data values are 7 and 5.)

| Address | Contents | Meaning |
|---------|----------|---------|
| 100 | Load 104 | Instruction 1 |
| 101 | Add 105 | Instruction 2 |
| 102 | Store 106 | Instruction 3 |
| 103 | Halt | Instruction 4 |
| 104 | 7 | Data: first number |
| 105 | 5 | Data: second number |
| 106 | (empty) | Space for the result |

### Activity

a. In the layout above, which addresses hold instructions, and which hold data?
b. Why does the program start at address 100 and not at address 0?

<details>
<summary><b>Answer</b></summary>

a. Instructions: **100 to 103**. Data: **104 to 106**.
b. Programs are loaded starting from a **predefined (chosen) address**. Here, 100 is the chosen starting point. The first instruction is placed there, and the PC is set to that address.

</details>

---

## Step 2: Fetching the Instruction (Fetch Cycle)

### Explanation

The CPU starts by **fetching** an instruction from memory. These registers work together:

| Step | What happens |
|------|--------------|
| 1 | The **PC** holds the address of the next instruction. At the start, it holds the address of the first instruction (for example, 100). |
| 2 | The PC value is **copied into the MAR**, to tell memory which address to read. |
| 3 | The instruction at that address is **copied from memory into the MBR**. |
| 4 | The instruction is **moved from the MBR to the IR**. |
| 5 | The **PC is increased by 1**, so it points to the next instruction. |

This increase by 1 makes sure that the CPU fetches the instructions **in order**.

[insert image about the fetch cycle: PC to MAR, memory to MBR, MBR to IR, then PC plus 1]

### Worked Example

**Task:** Trace the first fetch. The PC holds 100, and address 100 holds the instruction `Load 104`.

| Step | Register change |
|------|-----------------|
| 1 | PC = 100 |
| 2 | MAR = 100 (copied from the PC) |
| 3 | MBR = `Load 104` (read from memory address 100) |
| 4 | IR = `Load 104` (moved from the MBR) |
| 5 | PC = 101 (increased by 1) |

### Activity

The PC holds 101, and address 101 holds `Add 105`. Write the values of the PC, MAR, MBR, and IR after a full fetch.

<details>
<summary><b>Answer</b></summary>

- MAR = **101**
- MBR = **Add 105**
- IR = **Add 105**
- PC = **102** (increased by 1)

</details>

---

## Step 3: Decoding the Instruction (Decode Cycle)

### Explanation

When the instruction is in the IR, the CPU **decodes** it. In MARIE, each 16-bit instruction is split into two parts:

| Part | Size | What it does |
|------|------|--------------|
| **Opcode** | 4 bits | Says **which operation** to perform (for example Load, Add, or Subtract). *Opcode* is short for *operation code*. |
| **Address** (also called the **operand**) | 12 bits | Points to the **memory location** that holds the data |

The 12-bit address matches the memory size, because 2¹² = 4,096 locations.

In the standard MARIE instruction set, the main opcodes are:

| Instruction | Opcode (hex) | Opcode (binary) | What it does |
|-------------|--------------|-----------------|--------------|
| **Load X** | 1 | 0001 | Loads the data at address X into the AC |
| **Store X** | 2 | 0010 | Stores the AC's value at address X |
| **Add X** | 3 | 0011 | Adds the data at address X to the AC |
| **Subt X** | 4 | 0100 | Subtracts the data at address X from the AC |
| **Input** | 5 | 0101 | Reads a value from the InREG into the AC |
| **Output** | 6 | 0110 | Copies the AC into the OutREG |
| **Halt** | 7 | 0111 | Stops the program |

For example, with the instruction **Load 104**, the opcode tells the CPU to load data into the **AC**, and the address part (104) tells the CPU **which memory location** holds the data.

[insert image about the MARIE instruction format: a 4-bit opcode followed by a 12-bit address]

### Worked Example

**Task:** Write `Load 104` as a 16-bit instruction.

1. Opcode for Load = `0001`
2. Address 104 in hexadecimal = `0001 0000 0100` (1 = 0001, 0 = 0000, 4 = 0100)
3. Join them: `0001 0001 0000 0100`
4. In hexadecimal, this is **1104**

So the instruction stored in memory is **1104**. When the CPU decodes it, it sees opcode **1** (Load) and address **104**.

### Activity

Decode each instruction (write the operation and the address):

a. `3105`
b. `2106`
c. `7000`

<details>
<summary><b>Answer</b></summary>

a. Opcode 3 = **Add**, address **105**, so `Add 105`
b. Opcode 2 = **Store**, address **106**, so `Store 106`
c. Opcode 7 = **Halt** (the address part is not used)

</details>

---

## Step 4: Executing the Instruction (Execute Cycle)

### Explanation

After decoding, the CPU **executes** the instruction. Here is what happens for the main instructions:

**Load X**

1. The **MAR** is loaded with address X (taken from the instruction).
2. The data in memory at address X is fetched into the **MBR**.
3. The data moves from the **MBR** to the **AC**.

**Add X**

1. The **MAR** is loaded with address X.
2. The data at address X is fetched into the **MBR**.
3. The **ALU** adds the value in the **MBR** to the value in the **AC**, and the result is stored back in the **AC**.

**Store X**

1. The data in the **AC** moves to the **MBR**.
2. The **MAR** is loaded with address X, and the data in the **MBR** is **written** to memory at that address.

**Memory access**

- **Reading** from memory: the **MAR** holds the address, and the **MBR** receives the data from that address. Example: in a **Load**, the AC ends up holding the data that was fetched.
- **Writing** to memory: the data is first placed in the **MBR**, and the address in the **MAR**. The CPU then writes the data from the MBR to that address. Example: in a **Store**, the AC's data is written to memory.

**Arithmetic and logic in the ALU**

The ALU does the math. During **Add X**, the data at address X goes into the MBR, the ALU adds it to the AC, and the result goes back into the AC.

[insert image about the execute cycle for Load, Add, and Store, showing the registers MAR, MBR, AC, and the ALU]

### Worked Example

**Task:** Trace `Load 104` and then `Add 105`. Memory address 104 holds 7, and address 105 holds 5. The AC starts at 0.

**Load 104:**

| Step | Change |
|------|--------|
| MAR loaded with the address | MAR = 104 |
| Data read from memory into the MBR | MBR = 7 |
| Data moved to the AC | AC = 7 |

**Add 105:**

| Step | Change |
|------|--------|
| MAR loaded with the address | MAR = 105 |
| Data read from memory into the MBR | MBR = 5 |
| ALU adds MBR to AC | 7 + 5 = 12 |
| Result stored back in the AC | AC = 12 |

### Activity

The AC holds 12. Memory address 107 holds 20. Trace `Add 107`: what are the MAR, MBR, and AC afterward?

<details>
<summary><b>Answer</b></summary>

- MAR = **107**
- MBR = **20**
- ALU: 12 + 20 = 32, so AC = **32**

</details>

---

## Step 5: Input and Output, and the Halt Instruction

### Explanation

**Input and output**

MARIE uses two special registers to talk to the outside world:

| Register | Job |
|----------|-----|
| **InREG** (Input Register) | Holds the data received from an **input device** (for example, a keyboard) |
| **OutREG** (Output Register) | Holds the data to be sent to an **output device** (for example, a monitor) |

- **Input instruction**: The CPU reads the data from the **InREG** and loads it into the **AC**.
- **Output instruction**: The value in the **AC** is copied into the **OutREG** and sent to the output device.

**Halt instruction**

The **Halt** instruction **stops** the program. After Halt, the CPU **stops fetching and executing** instructions, so the program is finished.

[insert image about the Input and Output instructions moving data between the keyboard, InREG, AC, OutREG, and the monitor]

### Worked Example

**Task:** Trace a program with these instructions: `Input`, `Output`, `Halt`. The user types the number 9.

| Instruction | What happens | AC | OutREG |
|-------------|--------------|----|--------|
| Input | The 9 from the keyboard is in the InREG and is loaded into the AC | 9 | – |
| Output | The AC's value is copied to the OutREG and shown on the monitor | 9 | 9 |
| Halt | The program stops | 9 | 9 |

### Activity

a. Which register holds data that will be shown on the monitor?
b. What happens when the CPU executes a Halt instruction?

<details>
<summary><b>Answer</b></summary>

a. The **OutREG** (Output Register)
b. The CPU **stops fetching and executing** instructions, and the program ends.

</details>

---

## Case Study: Adding Two Numbers in MARIE

### Explanation

Now we put every step together. This program **adds two numbers** and stores the answer:

| Address | Instruction | What it does |
|---------|-------------|--------------|
| 100 | **Load 104** | The CPU sets the MAR to 104, fetches the data into the MBR, and moves it to the AC |
| 101 | **Add 105** | The CPU fetches the value at address 105 and adds it to the AC, and the result stays in the AC |
| 102 | **Store 106** | The CPU stores the AC's value into memory location 106 |
| 103 | **Halt** | The program ends, and no more instructions are run |

[insert image about the complete adding program flowing through the fetch, decode, and execute steps]

### Worked Example

**Task:** Trace the whole program. Address 104 holds 7, and address 105 holds 5. The PC starts at 100.

| Instruction | Fetch (PC → MAR → MBR → IR, PC + 1) | Decode | Execute | AC after |
|-------------|--------------------------------------|--------|---------|----------|
| 1 | PC = 100, IR = `Load 104`, PC becomes 101 | Opcode Load, address 104 | MAR = 104, MBR = 7, AC = 7 | 7 |
| 2 | PC = 101, IR = `Add 105`, PC becomes 102 | Opcode Add, address 105 | MAR = 105, MBR = 5, ALU: 7 + 5 | 12 |
| 3 | PC = 102, IR = `Store 106`, PC becomes 103 | Opcode Store, address 106 | MBR = 12, MAR = 106, memory[106] = 12 | 12 |
| 4 | PC = 103, IR = `Halt`, PC becomes 104 | Opcode Halt | The CPU stops | 12 |

**Result:** Memory address 106 now holds **12**, which is 7 + 5.

### Activity

Write a MARIE program (using Load, Subt, Store, and Halt) that works out **9 − 4** and stores the answer at address 106. Assume that address 104 holds 9 and address 105 holds 4. Then say what value ends up at address 106.

<details>
<summary><b>Answer</b></summary>

| Address | Instruction |
|---------|-------------|
| 100 | Load 104 |
| 101 | Subt 105 |
| 102 | Store 106 |
| 103 | Halt |

- Load 104 puts **9** in the AC.
- Subt 105 subtracts 4, so the AC becomes 9 − 4 = **5**.
- Store 106 writes the AC to address 106, so address 106 holds **5**.

</details>

---

## Stage 3 Summary

- **Program execution** is the computer carrying out a program's instructions, one after another, from the moment the program is in memory until it stops.
- **MARIE** is a simple model computer with three parts: the **CPU**, the **ALU**, and **memory** (4K words of 16 bits each).
- The CPU has a **datapath**, a **control unit**, and **registers**: **AC**, **PC**, **IR**, **MAR**, **MBR**, **InREG**, and **OutREG**.
- The program is **loaded into memory** first, starting at a set address.
- **Fetch**: PC → MAR → MBR → IR, then the PC goes up by 1.
- **Decode**: The instruction is split into a 4-bit **opcode** (the operation) and a 12-bit **address** (where the data is).
- **Execute**: **Load** moves data from memory to the AC, **Add** adds memory data to the AC using the ALU, and **Store** writes the AC to memory.
- **Input** and **Output** use the **InREG** and **OutREG**. **Halt** stops the program.
