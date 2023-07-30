# riscv_ctb_challenges
This repository contains the whole summary of hands on done by Abhinav Prakash (IS22MTECH14002) during the [RISC-V CTB 2023 Processor Design Verification Hackathon](https://community.riscv.org/events/details/risc-v-international-risc-v-academy-presents-risc-v-capture-the-bug-hackathon/) aims to introduce participants to the RISC-V ecosystem and familiarize them with the fundamentals of processor verification. Through this event, the RISC-V CTB imparts knowledge about the process of identifying bugs in RISC-V designs, emphasizing the importance of thorough processor verification.

![UPTICKPRO](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/b6ff3b02-fae6-4e9c-9752-b9106a441c1d)

# Table of Contents

# Level-1
## Challenge-1 logical
###  Identifying the Bug 
- To find the bug, we ran the `make` command and found the bug in 2 bugs.
- 
![Screenshot (2635)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/70a74152-9f35-4376-80f1-f636c3c9f650)

### Correcting the Bug
- To correct the bug, we replaced z4 with any of the defined registers in RV32I, like t0. So final instruction of line no 15855 in `test.S` file in `and s7,ra,t0`.
- Whereas in the next bug, `addi` performs addition with immediate data and s0 is not immediate data, so we replace s0 with any immediate data like 2. So final instruction of line no 25584 in `test.S` file in `addi s5,t1,2`.
- Then we run the make command, which generates `test.disass`,`test.elf` and `test_spike.dump` files.
  
![Screenshot (2642)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/d8984cea-ac4d-453d-bae4-8e6355040996)

## Challenge-2 logical
###  Identifying the Bug
- To find the bug we ran `make` command, and found the loop is running infinite times, so we came out of the loop using `Ctrl+c` and `q` and tried to find the bug.
  
![Screenshot (2645)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/8a9f5de9-c272-44b1-9476-a7f3f4a95685)

### Correcting the Bug
- We made the following changes in the code to run the loop properly.
 
![Screenshot (2646)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/7c9f23ac-5be7-4508-8703-6ff883e0957a)
- Finally, after running `make`, the required files were generated.

![image](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/481380cc-534c-44b8-a088-d0f0cb400c96)


## Challenge-3 illegal
###  Identifying the Bug
- To find the bug we ran `make` command and found the loop was running infinite times, so we came out of the loop using `Ctrl+c` and `q` and tried to find the bug.
  
![Capture](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/e009dffd-91cf-4a1e-b913-d9cfc5a6c5b6)
- We made the following changes in the code to run the loop properly.

![Screenshot (2660)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/b376fa14-62cd-47be-b3fb-b51293ec1422)

### Correcting the Bug
- Finally after running `make` the required files where generated.
  
![Screenshot (2653)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/11fe0c21-7235-446c-a216-2212d3e19664)

## Level-1 Refrences 
- [RISC-V Testing Environments - 1st RISC-V Bootcamp](https://www.youtube.com/watch?v=mbyb7BgYyXg)
- [rircv-test GitHub](https://github.com/riscv-software-src/riscv-tests)


# Level-2
## Challenge-1 instructions
###  Identifying the Bug 

### Correcting the Bug


## Challenge-2 exceptions
###  Identifying the Bug 

### Correcting the Bug



## Level-2 Refrences 
- [Automated Assembly Program Generator](https://gitlab.com/shaktiproject/tools/aapg)
- [Wiki AAPG](https://gitlab.com/shaktiproject/tools/aapg/-/wikis/Wiki-AAPG-%5B2.2.2%5D)







