# README — 6T and 8T SRAM Cells

**Project:** Design, Simulation & Verification of 6T and 8T SRAM Cells (Cadence Virtuoso, 45nm)

**Author:** Gokul Krish

**Target technology:** 45 nm CMOS process 



---

## 1. Introduction
This repository contains the complete transistor-level design and verification of **6T** and **8T Static Random-Access Memory (SRAM) cells** created using **Cadence Virtuoso** on a **45 nm CMOS technology node**.  
The project includes schematic design, ADEL simulations, physical layout creation, and verification through **DRC** and **LVS** checks. These SRAM cells demonstrate memory stability, read/write operation behavior, and physical design methodology used in modern VLSI design flows.

---

## 2. Schematics for 6T SRAM and 8T SRAM
- **6T SRAM Cell**  
  - Built using two cross-coupled inverters and two access transistors.  
  - Demonstrates typical SRAM read and write operation and cell stability.
 
    
<img width="1360" height="768" alt="Screenshot from 2025-11-17 18-59-11" src="https://github.com/user-attachments/assets/41ec95d1-4b76-41fe-89a3-d4f4c6d83ac9" />

 
    

- **8T SRAM Cell**  
  - Includes additional transistors for a separate read path.  
  - Improves read stability and avoids read-disturb problems.
 
    <img width="1360" height="768" alt="Screenshot from 2025-11-17 18-34-37" src="https://github.com/user-attachments/assets/404578e0-d2a8-4dc3-980c-684c3b59eda6" />


Both schematics are designed in **Cadence Virtuoso Schematic Editor** and validated through transistor-level simulation in **ADEL**.

<img width="1366" height="768" alt="6tSRAM" src="https://github.com/user-attachments/assets/adbe66b8-44e7-4d8c-9566-fedb8b2d081a" />

Simulation for 6T SRAM.


<img width="1848" height="1055" alt="8T_SRAM" src="https://github.com/user-attachments/assets/b2210beb-af33-4a2a-ab80-1f32da42707a" />

 Simulation for 8T SRAM


---

## 3. Layout for 6T SRAM and 8T SRAM
- Layouts are implemented in **Virtuoso Layout Suite** following 45nm PDK design rules.
- Key layout considerations:
  - Diffusion and poly sharing for area efficiency  
  - Bitline and wordline routing  
  - Metal layer optimization  
  - Proper well and implant placement  

Both cells are designed to be compact and ready for integration into larger memory arrays.

- **6T SRAM Cell** 
 
<img width="1360" height="768" alt="Screenshot from 2025-11-17 13-20-07" src="https://github.com/user-attachments/assets/c4a951b4-72f0-4977-8e6b-7ab56023464a" />


- **8T SRAM Cell**

  
<img width="1360" height="768" alt="Screenshot from 2025-11-17 18-34-30" src="https://github.com/user-attachments/assets/0cfe501a-fd9f-45c1-8f93-d0b322f44844" />

  

---

## 4. DRC and LVS for 6T SRAM and 8T SRAM
- **Design Rule Check (DRC)**  
  - Ensures the layout follows all geometric and spacing rules defined by the PDK.  
  - Both SRAM cell layouts pass DRC with zero violations.
 
  - **6T SRAM Cell**
    <img width="1360" height="768" alt="Screenshot from 2025-11-17 13-17-25" src="https://github.com/user-attachments/assets/39af8588-72d1-4d4a-8210-cb545c5baa6a" />



  - **8T SRAM Cell**
 <img width="1360" height="768" alt="Screenshot from 2025-11-17 18-32-22" src="https://github.com/user-attachments/assets/80836937-1a84-49a2-b706-288d8d9025e1" />

    
- **Layout vs Schematic (LVS)**  
  - Matches the layout-extracted netlist with the original schematic.  
  - Confirms correct connectivity and transistor matching.  
  - Both cells are **LVS clean** and verified for physical correctness.

  - **6T SRAM Cell**
  <img width="1360" height="768" alt="Screenshot from 2025-11-17 13-21-35" src="https://github.com/user-attachments/assets/5ce388d1-dd2b-4228-a7bf-bc3e79fdca41" />


  - **8T SRAM Cell**
  - <img width="1360" height="768" alt="Screenshot from 2025-11-17 18-33-33" src="https://github.com/user-attachments/assets/4383ea24-f2ef-452b-ae04-4a212f877797" />

    

---
