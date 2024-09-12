<p align="center">
  <a href="https://hcmus.edu.vn//" title="University of Science" style="border: none;">
    <img src="https://fetel.hcmus.edu.vn/wp-content/uploads/2022/09/logo-fetel.png" alt="University of Science">
  </a>
</p>

# Design of Two-Stage Opamp Circuit Using 90nm CMOS Technology

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/circuit.png)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/gain.png)

## Introduction

* This project is used as a final assignment for the VLSI Design course.
* The project is developed using Synopsys Custom Compiler, utilizing 90nm technology.
* The design of the Two-Stage Opamp follows specific requirements.
* It involves a full-flow custom IC design (schematic - simulation - layout - DRC, LVS checking).

### Supervisor

* MsC. Nguyen Thi Thien Trang - Faculty of Electronics and Telecommunications, University of Science - VNU-HCM

### Students Involved

|**No**|**Student ID**|  **Full Name**  |       **Email**      |
|------|---------------|------------------|----------------------|
|  1   |21207077       |Tran Thien Phuc   |21207077@hcmus.edu.vn |

## Project Execution

### Requirements to Execute the Project

* Synopsys Custom Compiler

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/custom_compiler.png)

* Design according to the provided specifications.

### Step 1: Follow the flow. Process specifications and calculate W/L

* Analyze the current mirror circuit using the Diode-Connected function.

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/current.png)

* Bring NMOS and PMOS into saturation (region 2).

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/diode.png)

* Survey the operating point to obtain the necessary parameters for calculating W/L of each stage.

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/OP.png)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/op1.png)

* After obtaining the parameters, begin calculations according to the specifications.

### Step 2: Draw schematic and symbol

* After calculating the necessary W/L, proceed to draw the schematic and symbol.

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/schematic.jpg)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/symbol.jpg)

### Step 3: Set up test benches for AC and transient simulations

* AC simulation test bench

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/testbench_ac.jpg)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/ac.jpg)

* Transient simulation test bench

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/testbench_trans.jpg)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/trans.jpg)

* After simulating the waveforms in AC and transient modes, the results show:
  
** In AC mode, the frequency and gain are close to the desired specifications.

** In Transient mode, the signal is amplified at Vout.

### Step 4: Draw layout, check DRC and LVS

* Layout image

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/layout.jpg)

* DRC check

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/drccheck.png)

For more info, check the project's report & ppt:
https://github.com/tthphuc1810/twostageopamp/blob/master/report/Two_Stage_Opamp_TTP.pdf
