# Sensorless FOC Motor Controller

**Electronics & Robotics Club, IIT Bombay**

This repository serves as the central hub for the development of a high-performance Sensorless Field-Oriented Control (FOC) ESC. It contains the technical roadmap, reference resources, hardware designs (KiCad), and firmware implementations.

## 📚 Technical Roadmap & Knowledge Base

### Phase 1: Theoretical Foundations
*Implementation of FOC requires a strong grasp of coordinate transformations. Blind implementation without understanding will result in suboptimal torque control.*

| Resource | Content |
| :--- | :--- |
| [TI Precision Labs - Motor Drivers](https://www.youtube.com/playlist?list=PLISmVLHAZbTQW1gK5ql0gq3HbwxF6BMjR) | BLDC Motor Physics & FOC Mathematics |


### Phase 2: Firmware Architecture & MCU Selection
*The system requires a microcontroller capable of high-frequency ADC sampling and real-time trigonometric calculations.*

| Resource | Content |
| :--- | :--- |
| [Phil's Lab: STM32 Mixed Signal Design](https://www.youtube.com/watch?v=v6fTa6LRJLI) | STM32G4 Hardware Architecture Overview |
| [SimpleFOC Documentation](https://docs.simplefoc.com/) | Control Library Structure & API |
| [VESC Project](https://vesc-project.com/) | Open Source ESC Reference Implementation |

### Phase 3: Hardware Design & PCB Layout
*The PCB requires a mixed-signal 4-layer design to minimize parasitic inductance and separate high-power switching noise from sensitive analog signal paths.*

| Resource | Content |
| :--- | :--- |
| [ST B-G431B-ESC1 Schematic (PDF)](https://www.st.com/resource/en/schematic_pack/mb1419-g431cbu6-c01_schematic.pdf) | **Reference Architecture.** Gate Driver & Current Sensing Schematics. |
| [TI: Designing with Motor Drivers](https://www.ti.com/video/series/precision-labs/ti-precision-labs-designing-with-motor-drivers.html) | Motor Controller Layout & Design Best Practices |
| [PCB Cupid (KiCad Workflow)](https://www.youtube.com/watch?v=szu8dJoyikA&list=PLn6004q9oeqGl91KifK6xHGuqvXGb374G) | KiCad Design Tutorials |

### Phase 4: Simulation & Tuning
*Prior to hardware integration, control loops must be validated in simulation.*

| Resource | Content |
| :--- | :--- |
| [SimpleFOCStudio](https://github.com/simplefoc/SimpleFOCStudio) | Real-time PID Tuning GUI |

---

## 🤝 How to Contribute Resources
If you find a new paper, video, or datasheet that is useful for the team:

1.  **Do not just drop a link in WhatsApp.**
2.  Edit this `README.md` file.
3.  Add the link to the **"Community Resources"** section below.
4.  Submit a Pull Request (or commit directly).

### 🔗 Community Resources (Added by Team)
*Add new links here in the format: `[Title](Link) - Description - @YourName`*
`[Motor Control from Scratch](https://youtube.com/playlist?list=PLl6mqZGq1o09k59iLGNs7AdLuJi9FoVcV&si=sy7RJGzMGQK_Qd8W) - PMSM motors, FOC, SVM - @Akshat Panda`
`[SENSORLESS FIELD ORIENTED CONTROL OF BRUSHLESS PERMANENT MAGNET SYNCHRONOUS MOTORS](https://krex.k-state.edu/server/api/core/bitstreams/e3f7aa0b-4833-44e4-9ef0-af09f411baa1/content) - Chapter 2,3,4, Appendix - @Akshat Panda`
`[Dynamic Model of PMSM motor and Torque](https://drive.google.com/file/d/1z1_R_sGhaGcJp3G0s5dLazDMSRDTJv_1/view?usp=sharing) - Rotating magnetic field, dq model of motor, Torque - @Akshat Panda`

* *Example: [Comparison of Inline vs Low-side Sensing](link) - Good article on why we chose inline - @TeamLead*
