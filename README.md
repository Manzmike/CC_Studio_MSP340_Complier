# Reason for Project
- As an Embedded Software Engineer/PCB Engineer with Embedded Experience, it is essential to be proficient in Embedded Engineering, especially when working with evaluation boards.
- Often, software requirements are provided before the PCB design is finalized.
- By prototyping software, most, if not all, design aspects can be completed in advance.
- In this case, the focus is on an evaluation board for devices.

# Design Programming for this Project
- This project involves creating a complete smart mirror that incorporates USB-C protocols with bare-metal programming.

# Requirements
- MSP430 Compiler from Texas Instruments

# Software Recommendations
What am I using?
- Code Composer Studio (CCStudio)
- MSP430 GCC Compiler
- macOS Operating System

# Hardware
- MSP430 TI Hardware Evaluation Kit

You can purchase the required evaluation kit on Amazon: [MSP430 Evaluation Kit](https://www.amazon.com/gp/product/B07J3R15JB/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1).

# Steps for Recreation
1. Open CCStudio.
2. Navigate to Devtools.
3. Select the hardware device most similar to your current hardware (for me, working on a MSP430 - EXP430G2ET).
4. Navigate back to CCStudio and under the Start Section, select "Browse and Import Examples".
5. Navigate to the `blink.c` under `/examples`, run the code to compile it.
6. Download the compiled code onto the board, either during the build or debug phase.
7. Run the code example on your board and observe the LED behavior change.
