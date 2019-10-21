# ND10_diskemu
A bus level disk emulator for the ND10/S

This project aims at creating a substitute for the ND-10/S SMD disk controller and SMD disk hardware due to the fact that it is 
very hard to get an old CDC SMD disk running, and keep it running.

The idea is to use the interface at the IO bus level replacing the entire controller and 1195 IO interface card by a Altera / Intel 
MAX 10 FPGA and STM32F407 uController. The choice of FPGA is based on the package type and the amount of pins available. The choice
of uController is based on the existance of a FSMC memory interface which will be used for communication with the ND-10/S through the 
FPGA and also the built in SDIO interface for use with SD cards.

[Google sheets with a breakdown of what is needed](https://docs.google.com/spreadsheets/d/1l8-pKSYi23ccKBfvMu0RAD9oF7giuxZcgCLQ8qeqaIM/edit?usp=sharing)



