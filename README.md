# RISC-V
## Digital Logic with TL-Verilog 
TL-X is a set of language constructs that can extend various Hardware Description Languages
(HDLs), including Verilog/SystemVerilog. Some combinational Circuits and Sequential Circuits Lab examples are discussed for the RISC-V architechture.
### 1) Combinational Circuits using TL-Verilog :
#### a) Inverter using TL-Verilog-
![Makerchip1 simple inverter combinational Circuit ](https://user-images.githubusercontent.com/97835399/155011208-1922a3fa-8e15-4d59-bcfc-03982678727f.png)
#### b) Arithmetic Operation using TL-Verilog-
The Input[3:0] is creates the array of vector of 5 bits.The bit ranges are not necessary for the RHS.

![Makerchip2 simple addition  combinational Circuit ](https://user-images.githubusercontent.com/97835399/155011502-6af87899-fbac-46b8-84dd-b990e13e6f41.png)

#### c)4X1 Multiplexer using TL-Verilog-

![Makerchip3 simple Multiplexer combinational Circuit ](https://user-images.githubusercontent.com/97835399/155011957-9ccb3664-0d65-438e-9c31-3946280621dd.png)

#### d) Combinational Calculator- 
The ciruit given below implements a Calculator that performs arithmetic operations on two input values.It consist of a 4X1 Mux to connected to output.

![image](https://user-images.githubusercontent.com/97835399/155012740-a385b898-7dfb-47dc-a2b8-e21ae9345e33.png)

![Makerchip4 (main) combinational Calculator](https://user-images.githubusercontent.com/97835399/155012798-b2fbe98f-a167-49c1-afa7-300d76aba8a6.png)

### 2) Seqential Circuits using TL-Verilog:
Sequential Logic is Sequenced by a cLock signal. 
#### a) Sequential Calculator using TL-Verilog-
The Combinational Calculator shown above is modified and the reset signal is added to the output which enables the calculator to perform new calculation each cycle.

![image](https://user-images.githubusercontent.com/97835399/155016679-13a2fc05-1f73-47a7-aeda-148b9377c45f.png)

![Makerchip5 simple counter   Sequential Calculator](https://user-images.githubusercontent.com/97835399/155016720-1cc65fe1-1561-4cb3-b3cd-08cebab3e627.png)
### 3) Pipelined logic:
A Large bit size Calculator won't work in high freqency operations because all the operations camnot fit in a clock period, for this reason we need pipeling in circuits, Pipeline logic is applied on the designed sequential calculator. 

#### a) Basic Circuit Implementation using TL-verilog:

![Pipeline Logic Makerchip ](https://user-images.githubusercontent.com/97835399/155019722-17693be5-a2bb-4829-a4d4-40747769c026.png)

#### b) Pipeline logic in the Calculator:

![image](https://user-images.githubusercontent.com/97835399/155020063-bdb3a77d-6a58-4084-8d85-df89cb213907.png)
![pipelining of main calculator ](https://user-images.githubusercontent.com/97835399/155868636-92a9faab-9c27-464e-a18c-c1e54b882e28.png)

#### b) Cycled Calculator with validity:
##### i)Validity-

Validity in TL-verilog is the notion when values of the signal is meaningful.The validity in TL-Verilog is expressed by 

$valid ..?

?$valid 

Due to the above argument the waveforms are much easier to interpret and the error checking gets easier.

##### ii) Clock gating:
Most of the power consumption of semiconductor device comes due the continuous clock distribution. The transition in the clock burns a lot of power. Clock gating avoids toggling of signals.

TL-verilog produce fined grade gating which can be enhanced by validity, this helps in knowing the valid signals and helps to reduce the clock gating.

In addition to this two more operation is added to the pipelined Calculator "mem" and "recall".

"mem" is going to capture the data into the memory 

"recall" is going to bring back the signal to the main calculator.

![image](https://user-images.githubusercontent.com/97835399/155873092-25a7eecc-3335-4a53-9b7d-0604f3b33991.png)
![image](https://user-images.githubusercontent.com/97835399/155856453-a76ef2a2-c974-4edf-acc1-d98254ba2193.png)

## RISC-V CPU Micro-architecture:

































