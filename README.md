# ARM-Processor
In this project we want to simulate ARM processor using Modelsim and Quartus. 

## Processor instruction set
<p align="justify"> The processor designed and implemented in this experiment is a simplified ARM processor that has 12 main instructions. This processor can perform mathematical operations (ADD, ADC, SUB, SBC), logical operations (AND, ORR, EOR) and comparison operations(CMP, TST), read and write operations in memory (LD, ST), and jump operations (B). The list of operations along with their details is given in the table below. The NOP command is not implemented as a command. </p>

![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/1f4bc94e-8e96-454d-b430-bdab0e49fa6c)

![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/73a5ea25-3053-4f57-ab71-9a45b3095616)

<p align="justify"> In ARM processors, all commands are executed conditionally. The following table lists the command execution modes. If a command is executed unconditionally, the condition bit value will be equal to 1110. If the condition is not met, the command will not do anything like NOP. </p>

![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/2cec825b-cb99-4994-8d31-c47898b74ee6)

For the shift operand in the ARM processor, it is implemented in the following three ways:

#### 32-bit immediate:
![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/217a7946-175f-4f3a-a111-db307276ce91)

#### Immediate shifts:
![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/6e849fa2-791c-4ff8-97a4-819595617bfe)

![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/1d250af2-622a-43df-95c6-224d9e00ca7c)

#### Register shifts:
![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/ac2a669d-a872-4aac-a087-1be2ac4a2317)

## Processor's Architecture
In this project we only consider forwarding unit and Hazard detection unit for our simulations. 

![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/117309ab-38ac-40fb-9782-04c0aef7e4a1)

![image](https://github.com/SogolGoodarzi/ARM-Processor/assets/125180530/12c8e4b7-5a3b-4bea-8926-aed753821aba)

<p align="justify"> So, by using pipeline model and the above block diagrams, we can create modules of different parts seperately and then properly connect them together to make the ARM processor. </p>
