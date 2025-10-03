# josephson-junction-transmon-experiments
Hands-on JJ→transmon mapping and calibration demos (Rabi/Ramsey) using Qiskit Aer with relaxation/dephasing noise.

# Josephson Junction → Transmon Qubit (Qiskit)

This repository contains a single, commented Jupyter cell that:

1) **Maps device → qubit**  
   Takes **critical current** \$(I_c$\) and **total shunt capacitance** \$(C_\Sigma$\) and computes:
   \$[
   E_J/h,\quad E_C/h,\quad f_{01}\approx\frac{\sqrt{8E_JE_C}-E_C}{h},\quad \alpha\approx-\frac{E_C}{h}.
   \$]
   This links **junction physics** (junction area/oxidation → \$(I_c$\); pads/geometry → \$(C_\Sigma $\)) to **qubit frequency** and **anharmonicity**.

2) **Runs standard control experiments**  
   In the \$(\{|0\rangle, |1\rangle\}$\) subspace:
   - **Rabi:** scan a resonant rotation angle \(\theta\) (pulse area) and measure \$(\langle Z\rangle$\).
   - **Ramsey:** \$(\pi/2$\) — wait \$(\tau $\) — \$(\pi/2 $\) with a programmed phase (detuning) to produce fringes that decay with \$(T_2^\* $\) (approximated here via a \$(T_2 $\) channel).







