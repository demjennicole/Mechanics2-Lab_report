# Moments of Inertia and Torsional Oscillations
 
Lab report for Mechanics II (Babeș-Bolyai University, Physics and Computer Science), written in LaTeX. The report itself is in Romanian.
 
Title in Romanian: *Momente de inerție și oscilații de torsiune*
Author: Nicole-Klarisza Demjen
 
## What this is about
 
The experiment studies a torsion axis (a rod on a torsion wire) in three parts:
 
1. Restoring torque. The rod is turned by 180 degrees from equilibrium and a dynamometer measures the force F needed to hold it, at a radius r = 0.1 m. The restoring torque constant is D = F r / pi.
2. Moment of inertia. The rod is turned by 90 degrees and released, and the time for 5 full oscillations is measured. From the period, J = D T^2 / (4 pi^2). Two masses are then placed symmetrically at different distances r, and the moment of inertia of each mass is J_c = (J - J_rod) / 2. A linear fit of J_c against r^2 (Steiner's theorem) gives the intrinsic moment of inertia of the body.
3. Damped oscillations. The decrease of the angular amplitude with the oscillation number is recorded.
## Main results
 
- Restoring torque constant: D = 0.02461 N m/rad
- Intrinsic moment of inertia (from the J_c(r^2) fit): J_0 = 1.98e-4 kg m^2
- Damped oscillations: the amplitude decreases roughly linearly with the oscillation number over the measured range, which indicates dissipation through friction.
See the report for the data tables, the plots and the discussion of error sources.
 
## Repository contents
 
- `main.tex` : LaTeX source of the report (rename to match your file)
- `figures/` : the images used in the report (`torsiune_1.jpg`, `torsiune_2.jpg`, `torsiune_3.pdf`, `torsiune_5.pdf`)
- `main.pdf` : compiled report
## Building the PDF
 
You need a LaTeX distribution (TeX Live or MiKTeX) with the Romanian `babel` option and the packages used in the preamble (`siunitx`, `booktabs`, `multirow`, `makecell`, etc.).
 
```
pdflatex main.tex
pdflatex main.tex
```
 
Run it twice so references resolve. The `\graphicspath` in the source points to `Mec. II/Laboratoare/`, so change it to `{figures/}` if you use the layout above.
 
## Notes
 
The plots were made in MATLAB. This is a student lab report, so the numbers come from a single measurement session and are affected by timing and reading errors, as discussed in the conclusion.
 
