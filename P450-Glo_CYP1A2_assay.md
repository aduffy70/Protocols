---
layout: page
title: P450-Glo CYP1A2 assay
categories: protocol
---

Adapted from [manufacturers protocol][1]

# General description

Measures cytochrome P450 CYP activity--specifically CYP1A2.

A proluciferin substrate provided in the kit (Luciferin-1A2) is acted upon by the CYP enzymes in the cultured cells to be tested to produce D-luciferin. Luciferin Detection Agent  provided in the kit is added to the cells, which lyses them and reacts with the released D-luciferin to produce light. More light = more D-luciferin = more P450 activity.

Because the light detection needs to happen in plates with black or white sided wells (not clear), either the cells need to be cultured in those plates (preferred method) or the lysate + Luciferin Detection Agent needs to be transfered from a normal culture plate to a black or white plate before measuring luminescence, taking care to transfer equal volumes for each well. Promega recommends white plates for highest luminescence readings, but black work for the range of luminescence we are seeing.

A standard curve should be generated to quantify how much light is produced by different amounts of D-luciferin. Make multiple dilutions from a known quantity of D-luciferin (Beetle D-luciferin, NOT provided with the kit), and react them with the Luciferin Detection Agent using the same concentrations/volumes as the experimental wells.

A No-cell control and vehicle controls (if some cells have been treated with AFB in DMSO, for example) are needed.

This version of the protocol should only be used on cells. Non-cell-based assays need additional reagents to jump-start the proluciferin/P450 reaction.

This CYP1A2 version needs PBS in place of media because the L-cysteine in media interferes with assays. The Substrate PBS for this version needs Salicylamide added to inhibit phase II conjugation of CYP products from CYP1A2/Luciferin-1A2. The Detection reagent for this version needs D-Cysteine to complete the conversion of the products to D-luciferin.


# Process

1. Start with cells cultured in 96 well plates, treated as desired (_e.g._, control vs AFB) for 24-72 hours.
1. Prepare Substrate PBS.
1. Remove media from cells and wash with PBS. Remove the PBS.
1. Add 50uL Substrate PBS to each cell well and control well.
1. Incubate at 37C 5% CO<sub>2</sub> for 30-60 minutes.
1. During incubation, prepare Luciferin Detection Reagent and Standard Dilutions.
1. Add 50uL of appropriate Standard Dilution to each standard well.
1. To each cell well, control well, and standard well add 50uL Luciferin Detection Reagent.
1. Mix briefly on a plate shaker to form lysate.
1. Read luminescence from plate using 1 second integration time (Promega recommends 0.25-1 second). Do not use a fluorometer and do not use filters with the luminometer.


# RECIPES

## Salicylamide stock
3M salicylamide in DMSO

  * 200 mg salicylamide
  * 350uL DMSO (Makes 500uL total)
  * Use immediately. Do not store.

## Substrate PBS
50uM Luciferin-1A2, 3mM salicylamide in PBS

Per well of a 96 well plate (multiply by number of cell wells and control wells plus 5-10% for pipette loss):
  * 0.05uL Luciferin-1A2 (provided with kit)
  * 0.05uL _fresh_ 3M Salicylamide stock
  * 49.90uL PBS
  * Use immediately. Do not store.

## Standard Dilutions
Beetle D-luciferin Potassium Salt in PBS at various concentrations:

### Stock Beetle Luciferin solution (2mM in water)

  * 5mg Beetle Luciferin Potassium Salt
  * 7.85mL mqWater
  * Aliquot and store in -80 freezer.

### Working Beetle Luciferin solution (80uM in PBS)

  * 20uL Stock Beetle Luciferin solution
  * 480uL PBS
  * Use this Working Beetle Luciferin solution to make 0, 0.032, 0.16, 0.8, and 4uM standard dilutions in PBS (see setup sheet). Note- those are the dilutions we make, but when the Detection Reagent is added later it will cut these concentrations in half, so the actual final concentrations for the standard curve are 0, 0.016, 0.08, 0.4, and 2uM.
  * Use immediately. Do not store.

## Luciferin Detection Reagent

  * Add entire bottle of reconstitution buffer (provided with kit) to amber bottle of lypholized Luciferin Detection Reagent (provided with kit).
  * Add 20uL D-Cysteine (in the kit)
  * Mix by swirling or inverting several times.
  * The reconstituted Luciferin Detection Reagent can be stored at room temperature for 24 hours or at 4C for 1 week without loss of activity. For long-term storage, store at –20°C for up to 3 months. Be sure to mix the thawed Luciferin Detection reagent well before use.

[1]: https://www.promega.com/-/media/files/resources/protocols/technical-bulletins/101/p450-glo-assays-protocol.pdf?la=en
