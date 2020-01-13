# Some things to understand about a microcontroller
Microcontroller consists of Program Memory (let’s call it Flash), SRAM, General Purpose Registers (GPR), IO Registers and Arithmetic Logic Unit (ALU).

A program is stored in Flash, it is persistent memory. A program consists of instructions. Each instruction consists of instruction code and one or more operands (in AVR there can be one or two operands, no more). Instruction code tells a processor of what actually to do, like add, subtract, compare, etc. And operands are data that operation is done on. During the execution of a program, you usually do not write to Flash(?).

SRAM, GPR and IO registers are not persistent, data is lost when power is off, but you can write to it and read from during execution of your program.

Arithmetic Logic Unit (ALU) is a block that can perform arithmetic and logical operations.
A program mainly does those arithmetic and logical operations, so when you write a program you want it to do those operations on some particular data.

The architecture of microprocessors is such, that it can perform arithmetic and logical operations only with data stored in GPRsor with operands in an instruction. So you have to put data into GPR or in instruction before you can apply arithmetic or logical operation on that data.
Also, there is a limit on how many GPR can be there, that’s also part of restrictions from hardware and architecture. So you can not store a large amount of data in those registers. That’s why you have to move data into GPR only when you need it, and move away when you don’t, so that you have a place for other data that you want to perform next operation on. 
When you move data away from GPR you place it in SRAM. It is usually much bigger than GPR and you can store much more data there. So the common workflow is the following:
* load from SRAM into GPR (into one or more registers)
* operate on those GPR
* store result in SRAM

Of Course, the program also has to do some IO operations: output something outside and read data from outside (input). For example, you want to transfer data to another device using some protocol or read data from other devices using some protocol; read data from a timer or configure that timer to do what you need. For that purpose there are IO registers, you can move data between those registers and GRPs or SRAM using particular instructions.

Also, programs usually have to behave differently depending on a particular condition. Those conditions are evaluated in ALU, and, depending on a result, you want to perform one or another part of your program. For this, particular instructions allow you to move to different parts of your program.
