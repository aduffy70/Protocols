---
layout: page
title: Quantifying DNA with Qubit
categories: protocol
---

Based on instructions from Hardeep Rai and updated for use in the Shaw lab

Equipment and supplies:
  * Dark storage in the drawer by the Qubit:
    * Qubit dsNDA HS buffer
    * Reagent/dye HS (light sensitive)
  * In the fridge:
    * HS standards (low and high)


1. Label clear 0.7mL tubes:
    * One for each sample
    * One for the low standard
    * One for the high standard
1. Mix enough working solution for samples, standards, and pipette loss. Vortex well and keep out of light. Per sample:
  * | Qubit dsDNA HS buffer | HS Qubit reagent |
    | --------------------- | ---------------- |
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
    * The number reported is the concentration in the tube being tested--NOT the concentration of the rest of your sample stock DNA! After reading the first sample, press the button to "Calculate Stock Conc" and set the amount of sample used (2uL).
    * Note the units reported and make necessary conversions to ng/uL. Once you know the conversion from the reported concentration to the stock concentration, you can just record the reported concentration and make the conversions yourself for the rest of the samples.
1. When finished, press Home to power down the Qubit. Dispose of tubes as normal lab waste
1. Return reagents to dark storage or the fridge as appropriate

Notes:
  * Using our normal 198:2 ratio, the HS (High sensitivity) will work for samples up to 60ng/uL. If the Qubit reports a sample is too high, rerun at 199:1 ratio, dilute the sample, or run with BR (Broad range) reagents with BR standards.
  * Standards must be run anytime the Qubit may have been used with a different dye (BR instead of HS).
  * See [this reference][1] for more information on why HS is limited to lower concentration samples.

[1]: http://www.epigenomes.ca/protocols-and-standards/quantifying-dna-samples-using-the-qubit-fluorometer-libpr-0030-ver-11.pdf
