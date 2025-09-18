# FEM Project – Torsion Analysis of Circular, Elliptical, and Triangular Sections  

## 📌 Project Overview  
This project investigates the torsional behavior of different cross-sections (circular, elliptical, triangular) using the Finite Element Method (FEM) in Abaqus.  
The aim is to study how geometry affects shear stress distribution, angle of twist, and warping phenomena under torsional loads.  

The project includes:  
1. Geometry creation for different cross-sections.  
2. Material property assignment (ASTM A36 steel).  
3. Mesh generation and verification.  
4. Application of torsional boundary conditions and loads.  
5. Extraction of stress, strain, displacement, and warping results.  
6. Validation and comparison of results across different sections.  

---

## 🎯 Objectives  
- Analyze torsional response of circular, elliptical, and triangular sections.  
- Study stress distribution and shear strain patterns.  
- Identify warping effects in non-circular sections.  
- Compare FEM results for different geometries.  
- Validate model accuracy with mesh convergence studies.  

---

## 🛠 Tools & Software  
- Abaqus/CAE – Geometry modeling, meshing, and FEM simulation.  
- Finite Element Method (FEM) – Numerical analysis of torsion.  
- ASTM A36 Steel – Material properties used for simulations.  

---

## 📐 Methodology  

### 1. Geometry Modeling  
- Created 3D deformable parts (circular, elliptical, triangular bars).  
- Added end grips to apply torsional loads uniformly.  

### 2. Material Properties  
- Used ASTM A36 steel.  
- Young’s Modulus = 210 GPa, Poisson’s Ratio = 0.3.  

### 3. Assembly & Boundary Conditions  
- Added grips at both ends of bars.  
- One end fixed, torsional rotation applied at the other end.  
- Two cases: +10 rad and -10 rad rotations.  

### 4. Meshing & Verification  
- Conducted mesh convergence studies.  
- Circular: optimal mesh = 40 seeds.  
- Elliptical: optimal mesh = 60 seeds.  
- Triangular: optimal mesh = 40 seeds.  

### 5. FEM Simulation (Abaqus)  
- Defined static general step.  
- Applied torsional loading via reference points and coupling constraints.  
- Solved using Abaqus standard solver.  

### 6. Post-Processing  
- Extracted von Mises stress, shear stresses (S13, S23), and displacement (U3).  
- Visualized deformed shapes and torsion-induced warping.  

---

## 📊 Results  
- Circular section: Uniform shear stress distribution, no warping.  
- Elliptical section: Non-uniform stress, warping observed due to asymmetry.  
- Triangular section: Highest stress concentration at sharp corners, strong warping.  
- Mesh convergence confirmed model validity.  

### Simulation Outputs  
- [Main Stress (Circular Section)](images/Circle.png)  
- [Main Stress (Elliptical Section)](images/Oval9.png)  
- [Main Stress (Triangular Section)](images/Triangle.png)  
- [Warping Visualization](images/Warping.png)  

---

## 📂 Repository Structure

├── Circle/ # Abaqus CAE/ODB files

├── Oval/ # Abaqus CAE/ODB files

├── Triangle/ # Abaqus CAE/ODB files

├── images/ # Simulation plots (stress, displacement, warping)

└── README.md # This file


---

## 🔬 Applications  
- Structural design of shafts, beams, and mechanical components.  
- Aerospace and automotive industries (torsional load analysis).  
- Educational use in Finite Element Method (FEM) and mechanics of materials.  
- Understanding warping effects in non-circular geometries.  

---

## 👨‍🎓 Authors  
- Mohammad Mahdi Khademi  
- Negar Naghavian  

Supervised by: Dr. Mohammad Javad Ashrafi  

Course: Introduction to Finite Element Method  

---

## 📖 References  
- Abaqus Documentation.  
- Shigley’s *Mechanical Engineering Design*.  
- Course lecture notes on FEM and torsion.
