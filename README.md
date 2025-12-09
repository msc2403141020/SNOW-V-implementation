# SNOW-V LFSR Components (Research Implementation)

This repository contains reference C implementations of the **LFSR-A** and **LFSR-B** components of the SNOW-V stream cipher.  
The code is written for research and teaching purposes as part of MSc coursework (MSC2403141020).

---

## 📌 Overview

SNOW-V is a modern high-performance stream cipher designed for 5G security.  
Its internal state consists of:

- **LFSR-A**: 256-bit linear feedback register over GF(2¹⁶), using the α and α⁻¹ mappings  
- **LFSR-B**: 256-bit linear feedback register over GF(2¹⁶), using the β and β⁻¹ mappings  
- **A combined update function**, which mixes both LFSRs
