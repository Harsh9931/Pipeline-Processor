# PIPELINE PROCESSOR

*COMPANY NAME* : CODTECH IT SOLUTION

*NAME* : HARSH PAWAR

*INTERN ID*  : CT08IQU

*DOMAIN* : VLSI

*BATCH DURATION* : January 5th, 2025 to February 5th, 2025

*MENTOR NAME* : NEELA SANTOSH

# DESCRIPTION

A 4-stage pipelined processor is a simple yet efficient design that enhances the execution speed of instructions by breaking down the instruction cycle into four sequential stages. This approach increases throughput by allowing multiple instructions to be processed simultaneously at different stages.

Designing a 4-stage pipelined processor with basic instructions (ADD, SUB, AND, LOAD) involves implementing the following pipeline stages:

Fetch (IF) – Fetches the instruction from memory.
Decode (ID) – Decodes the instruction and reads registers.
Execute (EX) – Performs arithmetic or logical operations.
Write Back (WB) – Writes results back to registers.
Pipeline Working Mechanism:

At every clock cycle, a new instruction enters the pipeline while previous instructions progress through their respective stages. This enables overlapping execution, where multiple instructions are executed in parallel, increasing efficiency. For example: At Cycle 1, ADD R1, R2 is fetched. At Cycle 2, ADD moves to decode while SUB R2, R3 is fetched. At Cycle 3, ADD moves to execute, SUB moves to decode, and AND R0, R1 is fetched. The process continues, with new instructions entering at each clock cycle.

# FUNCTIONAL DESIGN

The functional design of 4-stage pipelined processor can be described as follow:

Components Involved:

Instruction Memory – Stores instructions (ADD, SUB, AND, LOAD).
Register File – Holds general-purpose registers (R0-R3).
ALU (Arithmetic Logic Unit) – Executes arithmetic and logical operations.
Pipeline Registers – Store intermediate results between pipeline stages.
Control Unit – Manages instruction execution, ensuring proper sequencing.
Execution Flow Across Pipeline Stages Each instruction moves through four sequential stages, with multiple instructions executing simultaneously in different stages. The execution follows this order:

Instruction Fetch (IF) Action: Retrieves the instruction from memory.
In the simulation: Cycle 0: Fetch ADD
Cycle 5: Fetch SUB
Cycle 10: Fetch AND
Cycle 15: Fetch LOAD

Instruction Decode (ID) Action: Decodes the fetched instruction and reads operand registers.
In the simulation: Cycle 5:Decode ADD
Cycle 10: Decode SUB
Cycle 15: Decode AND
Cycle 20: Decode LOAD

Execution (EX) Action: Performs ALU operations or memory access.
In the simulation: Cycle 10: Execute ADD
Cycle 15: Execute SUB
Cycle 20: Execute AND
Cycle 25: Execute LOAD

Write Back (WB) Action: Writes the computed result back to the register file.
In the simulation: Cycle 15: Write ADD
Cycle 20: Write SUB
Cycle 25: Write AND
Cycle 30: Write LOAD

Analysis of Pipeline Execution Parallel Processing: Each stage operates on a different instruction, maximizing throughput.
Latency: Each instruction completes in 4 cycles, but new instructions enter the pipeline every cycle.
Pipeline Stalls: The "NOP" (No Operation) instructions appear after the last valid instruction, indicating pipeline completion.

Conclusion This project significantly enhanced my knowledge of Pipelined Processors and RTL coding. It reinforced the importance of simulation and verification in hardware design, particularly using Vivado. The insights gained from this project will aid me in future endeavors involving VLSI design and digital systems.

# TESTBENCH AND SIMULATION
![Image](https://github.com/user-attachments/assets/a800df7d-a2bf-44e0-9961-0a0ba632113e)
![Image](https://github.com/user-attachments/assets/90b69484-631c-4659-8170-ec8bc65d39aa)
