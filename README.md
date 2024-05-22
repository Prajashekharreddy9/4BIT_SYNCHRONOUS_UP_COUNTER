# 4BIT_SYNCHRONOUS_UP_COUNTER
# AIM
To stimulate and synthesis 4bit synchronous upcounter using Vivado

# Apparatus Required
vivado 2023.2 software.

# Procedure
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.


![image](https://github.com/RESMIRNAIR/4BIT_SYNCHRONOUS_UP_COUNTER/assets/154305926/4d676d34-2f12-420a-9c55-befa279f5ec0)
# Truth Table
# <img width="362" alt="image" src="https://github.com/RESMIRNAIR/4BIT_SYNCHRONOUS_UP_COUNTER/assets/154305926/2be84c5a-099f-4418-8d0b-ace34f734342">
# Timing diagram of the synchronous counter
![image](https://github.com/RESMIRNAIR/4BIT_SYNCHRONOUS_UP_COUNTER/assets/154305926/62c47758-b0a4-4fe0-842f-5c4245a88ff2)
# program
```
module synchronous_up_counter(

input wire clk, // Clock input

input wire reset, // Reset input

output reg [3:0] count // 4-bit output );

// Reset the counter to 0 when reset is active

always @(posedge clk or posedge reset)

begin

if (reset)

count <= 4'b0000;
else

count <= count + 1; // Increment the count on each clock cycle
end
endmodule
```
# output
![image](https://github.com/meghanareddy1006/4BIT_SYNCHRONOUS_UP_COUNTER/assets/163811142/a4c4a51a-d974-4f30-86d4-925b4f64a73e)
# result
Thus the verilog program for 4bit synchronous upcounter has been simulated and verified successfully.

