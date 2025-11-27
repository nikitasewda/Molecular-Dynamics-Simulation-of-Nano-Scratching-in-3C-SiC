# Molecular-Dynamics-Simulation-of-Nano-Scratching-in-3C-SiC
# Molecular Dynamics Simulation of Nano-Scratching and Burr Formation in 3C-SiC

This project investigates the nano-scratching behaviour of 3C-SiC (cubic silicon carbide) using Molecular Dynamics (MD) simulations. The objective is to understand how scratching depth and scratching velocity influence burr formation, chip morphology, subsurface damage (SSD), stress distribution, temperature rise, and atomic-scale phase transformation. The project is based on the complete 3C-SiC nano-scratching study provided in the uploaded document.

---

## Project Description

The work models a diamond abrasive tool scratching over a 3C-SiC workpiece and analyses the material removal behaviour at the atomic scale. The study focuses on:

- Exit burr formation
- Surface burr formation
- Chip height and width
- Subsurface damage (SSD)
- Tangential and normal force evolution
- Principal stress, Von Mises stress, and hydrostatic stress
- Temperature distribution during scratching
- Phase transformations analysed through RDF, Coordination Number (CN), and Common Neighbor Analysis (CNA)

Scratching depth is varied between 1–3 nm, and scratching velocity varies between 100–300 m/s. These parameters significantly affect the deformation behaviour, stress fields, thermal effects, and structural transformation within the SiC lattice.

---

## Objectives

- To study the effect of scratching depth on burr formation, chip generation, and subsurface damage.
- To analyse the influence of scratching velocity on burr dispersion, thermal agitation, and stress localisation.
- To evaluate cutting forces (Fx and Fz) during nano-scratching.
- To analyse stress evolution including principal stress, Von Mises stress, and hydrostatic stress.
- To quantify temperature rise at the tool–workpiece interaction zone.
- To investigate phase transformation using RDF, CN, and CNA to detect amorphization and lattice disorder.

---

## Simulation Setup

**Software Used**
- LAMMPS for MD simulation
- OVITO for visualization and post-processing

**Workpiece**
- Material: 3C-SiC
- Atoms: ~789,550

**Tool**
- Material: Diamond
- Shape: Spherical tip
- Radius: 8 nm
- Atoms: ~137,240

**Interatomic Potential**
- Tersoff potential for Si–Si, Si–C, and C–C interactions

**Boundary Conditions**
- Periodic in Y direction
- Non-periodic in X and Z directions

**Ensembles**
- NVT during equilibration
- NVE during scratching

**Simulation Parameters**
- Scratching depths: 1 nm, 2 nm, 3 nm
- Scratching velocities: 100 m/s, 200 m/s, 300 m/s
- Scratching distance: 20 nm
- Initial temperature: 300 K
- Time step: 0.5 fs

---

## Key Results

### Burr Formation
- Scratching depth is the most critical factor affecting burr generation.
- Bigger depths produce larger exit burrs and surface burrs.
- Higher velocity causes burrs to become more dispersed due to increased thermal agitation.

### Chip Morphology
- Chip height decreases with increasing velocity.
- Chip width increases with increasing velocity.
- Both height and width increase with scratching depth.

### Subsurface Damage (SSD)
- SSD thickness increases from ~30 Å (1 nm depth) to ~52 Å (3 nm depth).
- At higher velocities, SSD decreases due to reduced contact time.

### Stress Evolution
- First principal stress increases with both depth and velocity.
- Von Mises stress strongly depends on depth and weakly on velocity.
- Hydrostatic stress remains compressive beneath the tool.

### Temperature Distribution
- Peak temperatures range from approximately 1700 K to 2600 K depending on depth and velocity.
- Temperature rise is confined around the interaction region, preserving bulk structure.

### Phase Transformation
- RDF peaks decrease in intensity with increased depth and velocity, indicating loss of crystalline order.
- Coordination numbers shift from CN = 16 (crystalline) to CN = 12–14 (amorphous).
- CNA shows formation of amorphous and partially hexagonal structures in the SSD region.

---

## Significance of the Study

- Demonstrates atomistic mechanisms behind burr formation in hard-brittle ceramics.
- Shows the transition from brittle to ductile machining behaviour at nanoscale.
- Reveals how stress concentration, shear, and temperature govern chip formation.
- Provides a detailed understanding of subsurface lattice disruption.
- Useful for improving ultra-precision machining, wafer polishing, MEMS fabrication, and fine ceramic processing.

---

## Tools and File Structure (Suggested)


---

## How to Run

1. Install LAMMPS.
2. Place Tersoff potential files in `potential_files/`.
3. Run scratching simulation:
4. Visualize `.dump` files in OVITO.

---

## Conclusion

The MD simulations provide detailed atomistic insight into the nano-scratching behaviour of 3C-SiC. Scratching depth plays a dominant role in burr formation, chip generation, stress levels, temperature rise, and subsurface damage. Scratching velocity influences deformation localisation, thermal agitation, and burr dispersion. Phase transformation analysis shows amorphization and lattice disorder beneath the scratch groove. These findings contribute to the understanding of nanoscale machining of hard ceramic materials.

---

