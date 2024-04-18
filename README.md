# HALF_SUBTRACTOR
# Aim:
To simulate and synthesis Half Subtractaor using vivado.
# Apparatus Required:
Vivado Xilinx 14.7 Spartan 6 FPGA.
# Procedure:
```
STEP 1: Start the vivado software and select the name and the project.
STEP 2: Select the device family, device, package and speed.
STEP 3: Select new source in the new project and select verilog module as the source type.
STEP 4: Type the file name and module name and click next and then finish button. Type the code and save it.
STEP 5: Select the run simulation and then run behavioural simulation in the source window and click the check syntax.
STEP 6: Click the simulation to stimulate the program and give the inputs and verify the outputs as per the truth table.
STEP 7: Compare the output with the truth table.
```
# Truth Table
![image](https://github.com/RESMIRNAIR/HALF_SUBTRACTOR/assets/154305926/d0d5980a-6bcf-4ede-a54e-6aae3fb5f5f2)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/HALF_SUBTRACTOR/assets/154305926/df70da69-5a12-4a0d-ab84-a98dad3f7e70)
![image](https://github.com/RESMIRNAIR/HALF_SUBTRACTOR/assets/154305926/2f2d6a4d-9eda-4165-8579-1d7490b5fe97)
# Verilog Code:
```
module HS (a,b,difference,borrow);
input a,b;
output difference,borrow;
wire w1;
xor g1 (difference,a,b);
not g2 (w1,a);
and g3 (borrow,w1,b);
endmodule
```
# Output:
![halfsubtractor](https://github.com/GauravSunehl/HALF_SUBTRACTOR/assets/166976407/a23eb375-2ebe-4e58-83e1-42365a7d7395)
# Result:
Thus the verilog program for half subtractor has been simulated and verified successfully.

