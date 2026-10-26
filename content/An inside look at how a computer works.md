                        An inside look at how a computer works
   By the end of this chapter you will be able to answer:
 - How can a box of switches that can only count and store numbers be able to take the drudgery out of everyday mundane chores?
 - How can a computer shift through hundreds of thousands of possibilities and arrive at the best choice all within a few seconds?

   You will learn:
 - How information is identified inside a computer
 - Parts of a computer
 - How a processor works
 - How computer memory works
 - How information flows inside the computer


      A TOUR OF THE OUTSIDE
 	- Most of the components of a computer are contained inside the computer box, the computer case. Components visible from the outside:
         - Floppy Disk Drive (reads data from and writes data to floppy disks)
 - Used to store and transfer small amounts of data between computers.
 - Floppy disks can be inserted into the drive to access saved files or store new information.
         - CD-ROM Drive (reads data stored on compact discs)
- Used to install software, play music, or access files stored on CDs.
- CD-ROM stands for Compact Disc Read-Only Memory, meaning the data on the disc can be read but not modified.
         - Expansion Bays (provide space inside the computer case for additional hardware devices)
- Used to install extra drives, such as floppy disk drives, CD-ROM drives, or hard disk drives.
- They allow users to add or upgrade hardware according to their needs.
         - Power Switch 
(turns on the power)
- When a computer program goes astray, leaves you with no control (both the mouse and keyboard don’t respond to commands) 
The only recourse is to reboot by turning the power switch off and on.
         - Reset switch 
(refreshes the computer hardware without going through the full startup procedure)

      HOW INFORMATION IS IDENTIFIED
 - Computers encode information in terms of zeros and ones, bits and bytes. The components on the motherboard use this information to preform everyday tasks.
 - Information can be a person’s name, a bar code, or the number of the winning lottery ticket. Computers don’t grasp the way letters and numbers are written in any language, yet they are able to take and manipulate information, such as searching online.
 - Engineers bridged the gap between the method we use to identify information and the way computers identify information with the aid of the binary system, consisting of two digits, zero and one.
 - Each switch presents two states (off and on), where the flow of electricity is 
redirected from one circuit to another.
 - Binary value is used in calculations as much as it is in identifying the on and off 
position of a switch
 - Switches are arranged into logic circuits that are activated or deactivated based on the results of a calculation. 

      FROM BITS TO NUMBERS
 - A bit is a binary digit that has the value of zero or one, and a binary digit is a switch
 - The number 21 in binary form is 10101, holding 5 bits
 - A byte holds 8 bits of information

      FROM BITS TO LETTERS
 - Values up to 255 (the maximum size of a byte when converted to binary form) are distributed among the symbols and letters on a keyboard, called the ASCII (American Standard Code for Information Interchange)
 - Each letter and symbol has a specific number assigned to be converted into binary form. Then, with the help of a computer program, it’s binary form gets converted and displayed to the user.

      A TOUR OF THE INSIDE
 - One of the most important components inside a computer is the motherboard
 - circuit board that connects all the components.
         - Bus: Two or more wires that are usually etched into a circuit board over which \
information travels to components
-The most important component on the motherboard Is the CPU (Central Processor)
 - It’s the brain of the computer where all the computations occur, allows simultaneous execution of instructions. Computers that are used as servers and for other high-performance tasks sometimes use two or more CPU’s 
         - Memory chip: a large-scale integrated circuit used to store information
 - The most two common memory chips are ROM (read-only memory) and RAM (random access memory) 
1.ROM contains instructions and data that are etched into the chip. Information can’t be written or 
changed
- Tells the CPU how to load other programs such as the OS (Operating System)
2.RAM doesn’t hold any information 
         - Other examples include Video display cards, sound cards, modems, keyboards, and external ports 
 - A port is a receptacle that enables an external device to be connected to the motherboard. Information that flows to a printer travels within the wires etched into the motherboard from a processor to a port.
 - The power supply converts AC (alternating current) to DC (direct current) used to power the motherboard.
 - Components require specific voltage to interpret the signal that contains 
the binary number.
 - The clock circuitry pushes information between the CPU and the other 
components such as memory and ports. An easy analogy is to think the clock as sending pulsating waves, where each wave represents an instruction or data along wires etched into the motherboard.
 - A clock cycle is measured in megahertz (MHz); 1MHz is a million cycles per second, therefore, the higher the clock speed, the faster instructions and data will move within the computer.
 - The clock sets the speed outside of each component such as the processor. Often, other components run internally at a faster speed than the clock speed. 
 - For this reason, the clock is used to set a pace at which all components can operate efficiently.

      HOW A COMPUTER WORKS
 - The OS consists of more than one program; usually only one of those programs is 
running while the computer waits for a command. The other programs preform unique utility routines such as moving a command entered at the keyboard to the CPU for processing.
 - These utility programs are copied from hard-disks/floppy disks and stored in the 
memory ready to be used. Devices such as the keyboard, mouse, disk, drives, modems and devices connected to ports can request the CPU to process information through an uninterrupted request line (etched wires).
 - An interrupt is a message with priority over over current processes; makes other processes stop and run the program that is associated with the interrupt message.
The following three keys CTRL+ALT+DEL while a program is running are the panic keys on a Windows running computer. When the processes get stuck, this command enables you to shut down the processes.
   Process: 
1.Keyboard sends interrupt type value to the CPU
2.CPU realizes the interrupt type has higher priority and places the last instruction executed to a temporary memory before responding to the interrupt

      MOVING INSTRUCTIONS AND DATA INSIDE THE COMPUTER
 - One type of bus is an interrupt, as is the data bus used to transmit data within the computer.
Different bus types: 
1.IDE bus (connects the disk drives to the motherboard and the serial port, USB, etc.)
 - It’s a highway over which binary information encoded into small amounts of electricity travels
 - Binary values are encoded into the waves by changing the voltage:
 - two voltages, high and a low one represents a binary number of zero.  
Example: 3 volts might represent a binary one, while 2 volts a binary zero
 - Voltage regulators are responsible for maintaining specific voltages
 - Computer efficiency is measures as throughput
 - it rests in it’s architecture and the number of clock cycles, the size of the bus, the number of bits the CPU can process at one time and the internal processing power 

      MOVING DATA FROM THE OUTSIDE
 - Components within the computer are assigned a specific address along the bus. 
 - Each byte of memory has unique address, which is used by the processor to copy information from memory or send information to memory.
 - The expansion circuit board is connected to the bus on the motherboard 
by metallic finger-like strips (example: the USB has the metallic strips which plug in the motherboard)
 - Via a cable, serial ports connect a modem; The processor is instructed by a	
program to send a byte of information over to the modem; The byte flows from the CPU over the bus to the unique address of the serial port
 - In this case, the cable is bus of the serial port because the wires within the cable are used to communicate between the serial device and finally to the computer.

   INSIDE THE PROCESSOR
 - Three kinds of information are received by the processor:
         Interrupt message       Instructions      Data

 - Instructions are statements of a program written by a programmer that tell the processor to preform a specific task
Simple addition schematic
1.Access the specific memory address where the 1st number is stored and bring it to the processor
2.Store the 1st number in a register
 - Register is a small amount of memory located in the processor (used to store instructions and data temporary)  
3.Go to specific memory address where the 2nd number is stored and bring it to the processor
4.Copy both numbers from the registers to the arithmetic logic unit
5.Preform addition using those numbers
6.Move the sum to another register
7.Move the sum from the register to the video display adapter