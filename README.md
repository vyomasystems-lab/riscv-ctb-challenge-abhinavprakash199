# riscv_ctb_challenges
This repository contains the whole summary of hands on done by Abhinav Prakash (IS22MTECH14002) during the [RISC-V CTB 2023 Processor Design Verification Hackathon](https://community.riscv.org/events/details/risc-v-international-risc-v-academy-presents-risc-v-capture-the-bug-hackathon/) aims to introduce participants to the RISC-V ecosystem and familiarize them with the fundamentals of processor verification. Through this event, the RISC-V CTB imparts knowledge about the process of identifying bugs in RISC-V designs, emphasizing the importance of thorough processor verification.

![UPTICKPRO](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/b6ff3b02-fae6-4e9c-9752-b9106a441c1d)

# Table of Contents

# Level-1
## Challenge-1 logical
###  Identifying the Bug 
To find the bug we ran `make` command and find the bug in 2 bug ISA
![Screenshot (2635)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/70a74152-9f35-4376-80f1-f636c3c9f650)

### Correcting the Bug
- To correct the bug, we changed z4 with any of the defined registers in RV32I, like t0. So final instruction of line no 15855 in test.S file in `and s7,ra,t0`.
- Where as in the next bug, `addi` performs addition with immediate data and s0 is not immediate data, so we replace s0 with any immediate data like 2. So final instruction of line no 25584 in test.S file in `addi s5,t1,2`.
- Then we run the make command which generates `test.disass`,`test.elf` and `test_spike.dump` files.
![Screenshot (2642)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-abhinavprakash199/assets/120498080/d8984cea-ac4d-453d-bae4-8e6355040996)

## Challenge-2 logical
###  Identifying the Bug

### Correcting the Bug


## Challenge-2 illegal
###  Identifying the Bug

### Correcting the Bug





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







