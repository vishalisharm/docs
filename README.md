# ASSIGNMENT 1
## ADVANCE COMPUTER ARCHITECTURE

**Name:** Vishali  
**Roll No:** 26CS06018




## ASSIGNMENT 1(A)

| Benchmark      | Total # of Instructions | Load % | Store % | Uncond Branch % | Cond Branch % | Integer Computation % | Floating pt Computation % |
| -------------- | ----------------------: | -----: | ------: | --------------: | ------------: | --------------------: | ------------------------: |
| anagram.alpha  |              25,597,531 |  25.36 |    9.93 |            4.46 |         10.30 |                 44.63 |                      5.31 |
| go.alpha       |             545,823,141 |  30.62 |    8.17 |            2.58 |         10.96 |                 47.64 |                      0.03 |
| compress.alpha |                  88,204 |   1.58 |   79.17 |            0.20 |          5.71 |                 13.33 |                      0.00 |
| gcc.alpha      |                  51,126 |  16.31 |    4.82 |            3.74 |         13.74 |                 61.26 |                      0.06 |

### 1. ANAGRAM.alpha
![INPUT-OUTPUT](https://i.ibb.co/wF7KgRb0/Screenshot-2026-08-03-195659.png)


#### 1. Is the benchmark memory intensive or computation intensive?
- The percentage of load and store are 25.36, 9.93 so total percentage of memory instructions become 35.29%.
- The computation percentage of integer computation and floating point computation are 44.63,5.31 total percentage become 49.94%.
- Since almost 50% of the instructions are computational so anagram.alpha is computation intesive. 

#### 2. Is the benchmark mainly uses integer or floating point computations?
- Integer computations: 44.63% and Floating point computations: 5.31%, so it uses integer computations more.

#### 3. What % of the instructions executed are conditional branches?Given this %, how many instructions on average does the processor execute between each pair  of conditional branch instructions 
- percentage = 10.30%
- average instructions between conditional branches, 100/10.30 = 9.71, so on average 10 instructions.

### 2. GO.alpha
![INPUT-OUTPUT](https://i.ibb.co/Dg7d6Hcx/Screenshot-2026-08-03-194529.png)

#### 1. Is the benchmark memory intensive or computation intensive?
- The percentage of load and store are 30.62, 8.17 so total percentage of memory instructions become 38.79%.
- The computation percentage of integer computation and floating point computation are 47.64,0.03 total percentage become 47.67%.
- Since almost 50% of the instructions are computational so anagram.alpha is computation intesive. 

#### 2. Is the benchmark mainly uses integer or floating point computations?
- Integer computations: 47.64% and Floating point computations: 0.03%, so it uses integer computations more.

#### 3. What % of the instructions executed are conditional branches?Given this %, how many instructions on average does the processor execute between each pair  of conditional branch instructions 
- percentage = 10.96%
- average instructions between conditional branches, 100/10.96 = 9.12, so on average 9 instructions.


### 3. COMPRESS.alpha
![INPUT-OUTPUT](https://i.ibb.co/rf68Y9SD/Screenshot-2026-08-03-194633.png)

#### 1. Is the benchmark memory intensive or computation intensive?
- The percentage of load and store are 1.58, 79.17 so total percentage of memory instructions become 80.75%.
- The computation percentage of integer computation and floating point computation are 13.33,0.00 total percentage become 13.33%.
- Since almost 50% of the instructions are computational so anagram.alpha is memory intesive. 

#### 2. Is the benchmark mainly uses integer or floating point computations?
- Integer computations: 13.33% and Floating point computations: 0.00%, so it uses integer computations more.

#### 3. What % of the instructions executed are conditional branches?Given this %, how many instructions on average does the processor execute between each pair  of conditional branch instructions 
- percentage = 5.71%
- average instructions between conditional branches, 100/5.71 = 17.51, so on average 18 instructions.


### 4. GCC.alpha
![INPUT-OUTPUT](https://i.ibb.co/KcLn3G33/Screenshot-2026-08-03-194724.png)

#### 1. Is the benchmark memory intensive or computation intensive?
- The percentage of load and store are 16.31, 4.82 so total percentage of memory instructions become 21.13%.
- The computation percentage of integer computation and floating point computation are 61.26,0.06 total percentage become 61.32%.
- Since almost 50% of the instructions are computational so anagram.alpha is computation intesive. 

#### 2. Is the benchmark mainly uses integer or floating point computations?
- Integer computations: 61.26% and Floating point computations: 0.06%, so it uses integer computations more.

#### 3. What % of the instructions executed are conditional branches?Given this %, how many instructions on average does the processor execute between each pair  of conditional branch instructions 
- percentage = 13.74%
- average instructions between conditional branches, 100/13.74 = 7.28, so on average 7 instructions.


### ASSIGNMENT 1(B)

| AlphaBenchmarks| Total # of Instructions | Load % | Store % | Uncond Branch % | Cond Branch % | Integer Computation % | Floating pt Computation % |
| -------------- | ----------------------: | -----: | ------: | --------------: | ------------: | --------------------: | ------------------------: |
| test-math      |                  49,364 |  17.16 |   10.43 |            3.94 |         11.05 |                 55.38 |                      1.88 |
| test-fmath     |                  19,453 |  17.68 |   12.55 |            4.71 |         11.23 |                 53.24 |                      0.43 |
| test-llong     |                  10,581 |  17.74 |   14.66 |            5.44 |         12.32 |                 49.55 |                      0.10 |
| test-printf    |                 9,83,427|  17.99 |   10.73 |            4.82 |         11.39 |                 54.85 |                      0.09 |


| Pisa_Benchmarks| Total # of Instructions | Load % | Store % | Uncond Branch % | Cond Branch % | Integer Computation % | Floating pt Computation % |
| -------------- | ----------------------: | -----: | ------: | --------------: | ------------: | --------------------: | ------------------------: |
| test-math      |                2,13,745 |  15.96 |   10.66 |            4.22 |         13.85 |                 54.42 |                      0.88 |
| test-fmath     |                  53,504 |  16.14 |   14.41 |            4.24 |         15.11 |                 49.95 |                      0.11 |
| test-llong     |                  29,687 |  16.33 |   17.99 |            4.37 |         15.45 |                 45.82 |                      0.00 |
| test-printf    |                18,13,937|  19.22 |   09.28 |            5.13 |         17.01 |                 49.33 |                      0.01 |

### 1. Alpha 
#### - test-math 
![INPUT-OUTPUT](https://i.ibb.co/kV9h1VYD/Screenshot-2026-08-03-195122.png)
#### - test-fmath 
![INPUT-OUTPUT](https://i.ibb.co/BHXZGWWm/Screenshot-2026-08-03-195010.png)
#### - test-llong
![INPUT-OUTPUT](https://i.ibb.co/Xk532MF8/Screenshot-2026-08-03-194929.png)
#### - test-printf
![INPUT-OUTPUT](https://i.ibb.co/bjBnqTTK/Screenshot-2026-08-03-194834.png)

### Pisa
#### - test-math 
![INPUT-OUTPUT](https://i.ibb.co/67YBq6WH/Screenshot-2026-08-03-195503.png)
#### - test-fmath 
![INPUT-OUTPUT](https://i.ibb.co/Cshr4dfK/Screenshot-2026-08-03-195350.png)
#### - test-llong
![INPUT-OUTPUT](https://i.ibb.co/cXgG4KhV/Screenshot-2026-08-03-195229.png)
#### - test-printf
![INPUT-OUTPUT](https://i.ibb.co/1wTj8fW/Screenshot-2026-08-03-195555.png)


![INPUT-OUTPUT](https://i.ibb.co/q8x4Cvb/download.png)
![INPUT-OUTPUT](https://i.ibb.co/Q7xvwwXw/Screenshot-2026-08-03-193548.png)
![INPUT-OUTPUT](https://i.ibb.co/0RwcbwHT/Screenshot-2026-08-03-193654.png)
![INPUT-OUTPUT](https://i.ibb.co/dw5Mdtqq/Screenshot-2026-08-03-193800.png)
![INPUT-OUTPUT](https://i.ibb.co/XxBPXQrJ/Screenshot-2026-08-03-193848.png)
