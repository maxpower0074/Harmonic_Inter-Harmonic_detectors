# A Comparative Study of Harmonic and Inter-Harmonic Detection Using Parallel- and Cascade-Connected Nonlinear Limit Cycle Oscillators

## Authors

- Erick Vazquez
- Cesar-Fernando Mendez-Barrios

## Submission Information

**Submission ID:** 11047

---

## Description

The file **B2B_2x15kW_LCO_paralelo_y_serie.slx** is a MATLAB/Simulink model developed to reproduce the experimental results presented in the manuscript:

> *A Comparative Study of Harmonic and Inter-Harmonic Detection Using Parallel- and Cascade-Connected Nonlinear Limit Cycle Oscillators.*

The model implements both **parallel-connected** and **cascade-connected nonlinear limit cycle oscillator (LCO)** algorithms for harmonic and inter-harmonic detection in power systems.

To obtain the experimental results reported in the manuscript, the model must be executed using the hardware platform available at the **Smart Energy Integration Laboratory (SEIL), IMDEA Energy, Madrid, Spain**. The complete experimental setup and hardware specifications are described in the Experimental Section of the manuscript.

---

## Main Features

- MATLAB/Simulink implementation.
- Parallel-connected LCO harmonic and inter-harmonic detector.
- Cascade-connected LCO harmonic and inter-harmonic detector.
- Experimental validation on a 2 × 15 kW back-to-back converter platform.

---

## Requirements

- MATLAB R2024a or later.
- Simulink.
- Access to the SEIL experimental platform described in the manuscript.

---

## Installation

1. Copy the file:

   ```text
   B2B_2x15kW_LCO_paralelo_y_serie.slx
   ```

   into the MATLAB/Simulink environment.

2. Configure the experimental platform according to the hardware specifications provided in the Experimental Section of the manuscript.

3. Open the model in MATLAB/Simulink.

---

## Location of the LCO Detection Blocks

The Parallel and Cascade LCO implementations can be found at:

```text
VSC1 Controller2
 └── Grid Side Measurements
      └── D-LCO FLL
           └── Sequence Detection
```

---

## Model Execution

1. Open the main model:

   ```text
   B2B_2x15kW_LCO_paralelo_y_serie.slx
   ```

2. In the control interface, set the desired active and reactive power references:

   - `P_REF` : Active power reference
   - `Q_REF` : Reactive power reference

3. Start the converter by clicking:

   ```text
   Start_Load1
   ```

4. Connect the load by clicking:

   ```text
   Connect_Load
   ```

5. Once the system is operating, the harmonic and inter-harmonic components detected by the implemented LCO algorithms can be monitored through the corresponding measurement and visualization blocks.

---

## Notes

- This model is intended to reproduce the experimental results presented in the associated manuscript.
- The accuracy and reproducibility of the results depend on the use of the experimental hardware configuration described in the manuscript.
- Any modifications to the controller parameters or laboratory setup may affect detector performance and lead to results different from those reported in the paper.

---

## Citation

If you use this model in your research, please cite the associated manuscript:

**A Comparative Study of Harmonic and Inter-Harmonic Detection Using Parallel- and Cascade-Connected Nonlinear Limit Cycle Oscillators**

---

## Contact

For technical questions regarding the model or the experimental implementation, please contact the authors.