---
layout: page
title: Quantifying DNA with Qubit
categories: protocol
---

Based on instructions from Hardeep Rai and updated for use in the Shaw lab

Equipment and supplies:
  * Dark storage in the drawer by the Qubit:
    * Buffer solution
    * Reagent/dye HS (light sensitive)
  * In the fridge:
    * HS standards (low and high)


1. Label clear 0.7mL tubes:
    * One for each sample
    * One for the low standard
    * One for the high standard
1. Mix enough working solution for samples, standards, and pipette loss. Vortex well and keep out of light. Per sample:
  * | Qubit solution | HS Qubit reagent |
    | -------------- | ---------------- |
    | 199uL | 1uL |

1. Process standards and samples in batches of ~8 tubes to allow consistent timing.
1. To each standard tube add:
  * | Working solution | high or low standard |
    | ---------------- | -------------------- |
    | 190uL | 10uL |

1. Vortex well and let rest for 2 minutes.
1. Power on the Qubit by pressing ‘Go’
1. Select ‘dsDNA HS’
1. Follow the onscreen instructions to calibrate with the standards.
1. To each sample tube add:
  * | Working solution | DNA sample (gently pipette mixed) |
    | ---------------- | --------------------------------- |
    | 198uL | 2uL |

1. Vortex well and let rest for 2 minutes.
1. Follow the onscreen instructions to measure the samples.
    * After reading the first sample, arrow down to tell the machine we want the concentration and give it the amount of sample used (2uL)
    * The machine may provide readings in ug/mL, which is equivalent to ng/uL.
1. When finished, press Home to power down the Qubit. Dispose of tubes as normal lab waste
1. Return reagents to dark storage or the fridge as appropriate

Notes:
  * HS (High sensitivity) is for expected sample concentrations below about 100ng/uL. [This site][1] suggests that results above 70ng/uL are not accurate (the assay plateaus at ~100ng/uL and response is only linear below ~75ng/uL). If measured concentrations are higher than 70ng/uL dilute the sample and re-measure or use the BR (Broad range) reagents.
  * Standards must be run anytime the Qubit may have been used with a different dye (BR instead of HS).

[1]: http://www.epigenomes.ca/protocols-and-standards/quantifying-dna-samples-using-the-qubit-fluorometer-libpr-0030-ver-11.pdf
