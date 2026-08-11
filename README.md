
# ASSIGNMENT 2
## ADVANCE COMPUTER ARCHITECTURE
### NAME: Vishali
### ROLL NO. : 26CS06018

#### Objective : 
The objective of the assignmetn is to investigate the performance of a processor when different resources availability affect it. It uses the test-math benchmark. The experiment evaluates IPC, CPI,IPC Loss, Int Alu, Int Mul/Divsion , Fp Alu, Fp Mul/Division, Decode width, Issue width.
The test-math benchmark was executed using the SimpleScalar simulator. Here in this configuration A was used as the reference configuration.

#### Reference configuration used: 
- Fetch queue size = 4
- Decode width = 4
- Issue width = 4
- Commit width = 4
- In-order issue = true
- RUU size = 16
- LSQ size = 8
- Integer ALUs = 4
- Integer mult/div units = 4
- FP ALUs = 4
- FP mult units = 4
- Memory ports = 4

#### Formula Used to find IPC Loss:

$$
\text{IPC Loss (\%)} =
\frac{IPC_A - IPC_X}{IPC_A} \times 100
$$

## Observations- 
The reference configuration A executes 49,364 instructions in 78,198 cycles, giving an IPC of 0.6313 and CPI of 1.5841.

| Config | Changed Parameter | Value | Instructions | Cycles | IPC | CPI | IPC Loss from A (%) |
|---|---|---:|---:|---:|---:|---:|---:|
| A | Reference | - | 49364 | 78198 | 0.6313 | 1.5841 | 0.00 |
| B | Integer ALUs | 1 |49364  | 88866| 0.5555 | 1.8002 |  12.0070|
| B | Integer ALUs | 2 |49364  |79757  |0.6189  |1.6157  |1.9642  |
| B | Integer ALUs | 4 |49364  |78198  |0.6313  |1.5841 |  0.0000|
| C | Integer mult/div units | 1 |49364  |78198  |0.6313  |1.5841  |0.0000  |
| C | Integer mult/div units | 2 |49364  |78198  |0.6313 |1.5841  |0.0000  |
| C | Integer mult/div units | 4 |49364  |78198  |0.6313  |1.5841  |0.0000  |
| D | FP ALUs | 1 |49364  |78209  |0.6312  |1.5843  |0.0158  |
| D | FP ALUs | 2 |49364  |78201  |0.6312  |1.5842  |0.0158  |
| D | FP ALUs | 4 |49364  |78198  |0.6313 |1.5841  |0.0000  |
| E | FP mult units | 1 |49364  |78208  |0.6312  |1.5843  |0.0158  |
| E | FP mult units | 2 |49364  |78198  |0.6313  |1.5841  |0.0000  |
| E | FP mult units | 4 |49364  |78198  |0.6313  |1.5841  |0.0000  |
| F | Memory ports | 1 |49364  |78198  |0.6313  |1.5841  |0.0000  |
| F | Memory ports | 2 |49364  |78198  |0.6313  |1.5841  |0.0000  |
| F | Memory ports | 4 |49364  |78198  |0.6313  |1.5841  |0.0000  |
| G | Decode width | 1 |49364  |94686  |0.5213  |1.9181  |17.4244  |
| G | Decode width | 2 |49364  |81095  |0.6087  |1.6428|  3.5799|
| G | Decode width | 4 |49364  |78198  |0.6313  |1.5841  |0.000  |
| H | Issue width | 1 |49364  |89408  |0.5521  |1.8112  |  12.5455|
| H | Issue width | 2 |49364  |79883  |0.6180  |1.6182  |  2.1068|
| H | Issue width | 4 |49364  |78198  |0.6313  |1.5841  |  0.0000|
| J | RUU size | 8 |49364  |78344  |0.6301  |1.5871  |0.1901  |  
| J | RUU size | 16 |49364  |78198  |0.6313  |1.5841  |  0.0000|

## OBSERVATION 
1. Integer ALU: In the reference one we have 78,198 cycles which increase when we decrease the number of integer alu,
   when we increase to 2 the ipc become 0.6139 and in the case of  int alu 1 the cycles increase upto 88k with 0.555 ipc.
2. Integer MUL: In this one even when we change the number of integer multpy/divide units to 2 and 1 the configurations remain same
   as that of the reference and nothing much changes.
3. Fp ALU: This one has negligible effect on the ipc or the number of cycles with 1 fpalu, the cycles has slight increase upto 78,209 with ipc
   slightly decreasing upto 0.6312 and even with 2fpalu same effect is seen.
4. Fp MUL: This one also has negligible effect with 2 fpmul we are only getting the same configuration as of the reference and with 1 fp mul units the cycles
   slightly increase to 78,208 producting ipc loss of 0.0158%.
5. Memory Ports: Configurations with 1,2,4 all shows the same as reference configuration with loss ipc of 0% in every case. The observation
   made is that memory ports does not constrain the workload.
6. Decode Width: With decode width of 1, cycles drastically increase upto 94k and ipc falls upto 0.5213, resulting in 17% of ipc loss.
   Increasing the decode width to 2 improves the performace where cycles falls upto 81k and ipc increases to 0.6087.
7. Issue Width: With issue width of 1, cycles drastically increase upto 89k and ipc falls upto 0.55, resulting in 12% of ipc loss.
   Increasing the decode width to 2 improves the performace where cycles falls upto 79k and ipc increases to 0.6180.
8. Ruu size: with 8 ruu size the cycles increase slightly to 78,344 and ipc decreases to 0.6301 giving only 0.2% loss. It has only minor effect.
## PLOTS 
![INPUT-OUTPUT](https://i.ibb.co/xKZhGJPh/Integer-ALUs.png)
![INPUT-OUTPUT](https://i.ibb.co/WpPKCW2V/FP-ALUs.png)
![INPUT-OUTPUT](https://i.ibb.co/tw1pVGpv/Integer-mult-div-units.png)
![INPUT-OUTPUT](https://i.ibb.co/vxk1sJhX/FP-mult-units.png)
![INPUT-OUTPUT](https://i.ibb.co/jZ3T2CB9/Decode-width.png)
![INPUT-OUTPUT](https://i.ibb.co/TMZQKF15/Issue-width.png)
![INPUT-OUTPUT](https://i.ibb.co/B2NkqVK1/Memory-ports.png)
![INPUT-OUTPUT](https://i.ibb.co/0pJzcdpK/RUU-size.png)
