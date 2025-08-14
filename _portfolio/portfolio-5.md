---
title: "5V to 3.3V LDO Project"
excerpt: "Personal Project <br/><br><img src='/images/ldo_layout.png' width='50%' height='50%'>"
collection: portfolio
---

This is a personal project I've been recently working on. I'm designing a 5V to 3.3V low dropout regulator using the Cadence GPDK, which takes in a noisy power input and outputs a steady DC voltage. LDOs are a fundamental block of analog IC design and see frequent use in providing stable power to other circuits on-chip. Circuit layouts and specs are shown below. Results are also compared to the [LM3940](https://www.ti.com/lit/ds/symlink/lm3940.pdf?ts=1754872909603) designed by Texas Instruments.

![](/images/ldo_layout_labeled.png)

All specs are at 25 degrees C with both circuits operating in the same conditions

| Spec                | This Work                             | LM3940                                |
| PSRR                | 10kHz: 28dB, 100kHz: 42dB, 1MHz: 68dB | 10kHz: 35dB, 100kHz: 30dB, 1MHz: 29dB |
| Quiescent Current   | 1.25mA                                | 10mA                                  |
| Output Voltage      | 3.3V                                  | 3.3V                                  |
| Dropout Voltage     | 13.6mV                                | 100mV                                 |
| Output Resistance   | 35 Ohms                               | 0.05 Ohms                             |  
| Peak Output Current | 100mA                                 | 1.5A                                  |

[Appendix](/portfolio/portfolio-5/appendix)
