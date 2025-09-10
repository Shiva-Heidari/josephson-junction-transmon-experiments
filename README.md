# josephson-junction-transmon-experiments
Hands-on JJ→transmon mapping and calibration demos (Rabi/Ramsey) using Qiskit Aer with relaxation/dephasing noise.

# JJ → Transmon Lab (Qiskit)

From **Josephson junction (JJ) device parameters** to **transmon qubit experiments** in one notebook.  
This repo computes \$(E_J, E_C, f_{01}$\), and anharmonicity \$(\alpha$\) directly from \$((I_c, C_\Sigma) $\), then runs **Rabi** and **Ramsey** experiments in **Qiskit Aer** with a simple \$(T_1/T_2 $\) noise model.

---

## Why this is useful
- Shows the **device → qubit** mapping (junction physics to qubit frequency & nonlinearity).
- Demonstrates standard, interview-familiar experiments (**Rabi**, **Ramsey**) with code you can run end-to-end.
- Clean, minimal dependencies; easy to extend (Shapiro steps, SQUID flux tuning, transmon diagonalization).

---

## Contents
- `README.md` (this file)
- `transmon_from_jj_rabi_ramsey.ipynb` *(notebook name suggestion)*  
  A single notebook with:
  1) markdown primer (JJ → transmon theory),  
  2) a commented Python cell that:
     - maps \$ ((I_c, C_\Sigma) $\) → \$(E_J/h$\), \$(E_C/h$\), \$(f_{01}$\), \$(\alpha $\)  
     - builds **Rabi** and **Ramsey** circuits in Qiskit  
     - simulates with **thermal relaxation** noise (set \$(T_1, T_2 $\))  
     - plots \$(\langle Z\rangle$\) vs drive angle (Rabi) and vs delay (Ramsey)




