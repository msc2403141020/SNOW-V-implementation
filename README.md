# SNOW-V Full Model Implementation (Research Work)

This repository contains a full C implementation of the SNOW-V stream cipher, including:
- LFSR-A and LFSR-B (256-bit each, over GF(2¹⁶))
- FSM (Finite State Machine)
- Complete initialization and keystream generation
- Verification with test vectors from the SNOW-V specification

The code is developed for research purposes as part of my MSc Research Project.


## 📌 Overview

SNOW-V is a modern high-speed stream cipher designed for 5G/6G security.
This implementation includes all core components:

✔ LFSR-A
~ Operates using α and α⁻¹ mappings
~ 16 × 16-bit cells
~ Implements polynomial 0x990F and inverse 0xCC87

✔ LFSR-B
~ Operates using β and β⁻¹ mappings
~ 16 × 16-bit cells
~ Implements polynomial 0xC963 and inverse 0xE4B1

✔ FSM (AES-like round function)
~ Implements Sigma permutation
~ Uses S-Box lookups
~ Operates on R1, R2, R3 registers

✔ Complete SNOW-V Full Model
~ Accepts 32-byte key and 16-byte IV
~ Performs the 16-round warm-up initialization
~ Generates 128-bit keystream blocks

Output verified against the official test vectors from the paper
(the code output matches exactly).
