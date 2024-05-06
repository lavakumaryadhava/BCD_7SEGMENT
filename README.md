# AIM
To design and simulate BCD 7 Segment using Vivado 2023.2.
# Software Required:
vivado 2023.2 software.

# Procedure:
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table
# BCD_7SEGMENT
![image](https://github.com/RESMIRNAIR/BCD_7SEGMENT/assets/154305926/804ab8db-8637-45ac-b10f-80e77d818d61)
# PROGRAM
```
module segment7(
     bcd,
     seg
    );
     
     
     input [3:0] bcd;
     output [6:0] seg;
     reg [6:0] seg;
    always @(bcd)
    begin
        case (bcd) //case statement
            0 : seg = 7'b0000001;
            1 : seg = 7'b1001111;
            2 : seg = 7'b0010010;
            3 : seg = 7'b0000110;
            4 : seg = 7'b1001100;
            5 : seg = 7'b0100100;
            6 : seg = 7'b0100000;
            7 : seg = 7'b0001111;
            8 : seg = 7'b0000000;
            9 : seg = 7'b0000100;
            
            default : seg = 7'b1111111; 
        endcase
    end
    
endmodule
```
# OUTPUT
![image](https://github.com/lavakumaryadhava/BCD_7SEGMENT/assets/162088994/dde9d2ce-519c-453e-a358-4c36c813f531)

# Result:
Thus the BCD 7 Segment is verified successfully.

