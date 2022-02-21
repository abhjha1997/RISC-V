# RISC-V
## Digital Logic with TL-Verilog 
TL-X is a set of language constructs that can extend various Hardware Description Languages
(HDLs), including Verilog/SystemVerilog. Some combinational Circuits and Sequential Circuits Lab examples are discussed for the RISC-V architechture.
### Combinational Circuits using TL-Verilog :
#### 1) Inverter using TL-Verilog-
![Makerchip1 simple inverter combinational Circuit ](https://user-images.githubusercontent.com/97835399/155011208-1922a3fa-8e15-4d59-bcfc-03982678727f.png)
#### 2)Arithmetic Operation using TL-Verilog-
The Input[3:0] is creates the array of vector of 5 bits.The bit ranges are not necessary for the RHS.

![Makerchip2 simple addition  combinational Circuit ](https://user-images.githubusercontent.com/97835399/155011502-6af87899-fbac-46b8-84dd-b990e13e6f41.png)

#### 3) 4X1 Multiplexer using TL-Verilog-

![Makerchip3 simple Multiplexer combinational Circuit ](https://user-images.githubusercontent.com/97835399/155011957-9ccb3664-0d65-438e-9c31-3946280621dd.png)

#### 4) Combinational Calculator-
The ciruit given below implements a Calculator that performs arithmetic operations on two input values.It consist of a 4X1 Mux to connected to output.

![image](https://user-images.githubusercontent.com/97835399/155012740-a385b898-7dfb-47dc-a2b8-e21ae9345e33.png)

![Makerchip4 (main) combinational Calculator](https://user-images.githubusercontent.com/97835399/155012798-b2fbe98f-a167-49c1-afa7-300d76aba8a6.png)

### Seqential Circuits using TL-Verilog:
Sequential Logic is Sequenced by a cLock signal. 
#### 1) Sequential Calculator using TL-Verilog-
The Combinational Calculator shown above is modified and the reset signal is added to the output which enables the calculator to perform new calculation each cycle.

![image](https://user-images.githubusercontent.com/97835399/155016679-13a2fc05-1f73-47a7-aeda-148b9377c45f.png)

![Makerchip5 simple counter   Sequential Calculator](https://user-images.githubusercontent.com/97835399/155016720-1cc65fe1-1561-4cb3-b3cd-08cebab3e627.png)
### 3) Pipelined logic:
A Large bit size Calculator won't work in high freqency operations because all the operations camnot fit in a clock period, for this reason we need pipeling in circuits, Pipeline logic is applied on the designed sequential calculator. 

#### ) Basic Circuit Implementation using TL-verilog:

![Pipeline Logic Makerchip ](https://user-images.githubusercontent.com/97835399/155019722-17693be5-a2bb-4829-a4d4-40747769c026.png)

#### ) Pipeline logic in the Calculator:



![image](https://user-images.githubusercontent.com/97835399/155020063-bdb3a77d-6a58-4084-8d85-df89cb213907.png)


























