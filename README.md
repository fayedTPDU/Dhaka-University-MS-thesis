# Quantum K-Means for Jet Clustering at Hadron Colliders like LHC
**MSc Thesis Project – Theoretical & Computational Particle Physics**

This repository hosts the **research overview, documentation, and selected results** from my Master’s thesis, where I explore the use of **Quantum Machine Learning (QML)**—specifically **Quantum K-Means (QK-Means)**—for jet clustering in proton–proton collision events from the **Large Hadron Collider (LHC)**.

---
 **Project Summary**

High-energy particle collisions produce collimated sprays of particles called **jets**, and jet clustering is an essential task for event reconstruction in collider physics.  

Classical clustering algorithms such as **K-Means** or **Anti-\(k_t\)** scale poorly with increasing dataset size. Quantum algorithms offer promising computational advantages due to:

- Amplitude encoding  
- High-dimensional Hilbert space representation  
- Potential sublinear distance computation  

This thesis investigates whether **Quantum K-Means** (implemented using Qiskit’s QASM simulator) can provide **runtime or scaling benefits** over classical methods.

---

## **Key Components of This Project**

### **1. Quantum K-Means Design**
- Implementation of QK-Means using:
  - Quantum distance estimation
  - Quantum feature encoding
  - A hybrid quantum–classical update loop
- Simulations performed using **IBM Qiskit Aer**.

### **2. Classical Baseline**
- Classical K-Means implemented in NumPy.
- Runtime comparison with matched dataset dimensions.
- Synthetic and LHC-style 4-momentum data used.

### **3. Datasets**
- **Synthetic 4-vector datasets** (toy MC).
- **LHC-style real dataset** (`realdata.txt`) containing:
  - Energy \(E\)
  - Momentum components \(p_x, p_y, p_z\)
  - Derived quantities (η, φ, pT)

### **4. Runtime Experiments**
Runtime scaling was tested for multiple dataset sizes (e.g., 12, 29, 45, 62…).  
Noise-free simulations were used to isolate algorithmic scaling behavior.

---

##  **Results Overview**

- Quantum K-Means shows **competitive or slightly better simulation runtime** than classical K-Means for small dataset sizes, due to parallelizable distance operations in the simulator.
- Runtime still depends on simulator parameters and does _not_ reflect hardware execution time.
- The results demonstrate feasibility but not yet quantum advantage — hardware limitations remain significant.

Full plots, complexity analysis, and conclusions are included in the thesis document.

---

## 🚫 **Code Availability**

**The complete source code for this project is currently not included in this repository.**

I intend to publish this work in a peer-reviewed venue, and releasing the full implementation **before publication** may affect the novelty and integrity of the submission.

For this reason:

- Selected figures  
- Runtime tables  
- Documentation  
- Thesis PDF  

…are provided here, but the **core algorithmic code** (Quantum K-Means and dataset processing pipeline) will be made public **after publication**.

If you are a researcher and would like to collaborate or review the methods, feel free to contact me.

---

## 📁 Repository Structure
