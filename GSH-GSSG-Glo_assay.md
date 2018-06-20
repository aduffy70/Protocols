---
layout: page
title: GSH/GSSG-Glo assay
categories: protocol
---

Adapted from [manufacturers protocol][1]

# General description

Measures quantities of GSH and GSSG (cofactors for GSTs) present in cultured cells.

We measure Total Glutathione (GSH and GSSG) and Oxidized Glutathione (GSSG only). Subtracting GSSG from Total Glutathione gives the amount of GSH.

The Total Glutathione assay works by lysing the cells and reducing GSSG to GSH with Total Glutathione Lysis Reagent (provided in the kit) so all the Glutathione is GSH. Then the GSH and a Luciferin Generation Reagent (provided) are acted upon by GST (provided) producing Luciferin. Luciferin Detection Reagent (provided) reacts with the Luciferin to produce light. More light = More Luciferin = More GSH and GSSG.

The GSSG-only assay works similarly, but uses a Oxidized Glutathione Lysis Reagent (provided) that lyses the cells and blocks the GSH present in the cells, leaving only the GSSG to be converted to GSH. The rest of the assay is the same as above. More light = More Luciferin = More GSSG.

Because the light detection needs to happen in plates with black or white sided wells (not clear), either the cells need to be cultured in those plates (preferred method) or the lysate + Luciferin Detection Agent needs to be transfered from a normal culture plate to a black or white plate before measuring luminescence, taking care to transfer equal volumes for each well. Promega recommends white plates for highest luminescence readings, but black work for the range of luminescence we are seeing.

A standard curve should be generated to quantify how much light is produced by different amounts of GSH using the Total Glutathione assay. Make multiple dilutions from a known quantity of GSH (provided with the kit), and run them through the entire assay process.

A vehicle control (if some cells have been treated with AFB in DMSO, for example) is needed for both assays. A No-cell control only needs to be run for one of the assays (and the zero glutathione reactions of the standard curve serve as the no-cell controls)

This assay is sensitive so it requires fewer cells per plate than other assays, but our normal plating technique gave luminescence levels in the linear portion of the standard curve.

# Process

1. Start with cells cultured in 96 well plates, treated as desired (_e.g._, control vs AFB) for 24-72 hours.
1. Prepare Total Glutathione Lysis Reagent, Oxidized Glutathione Lysis Reagent, and Standard Dilutions.
1. Remove media from cells.
1. Add 5uL of appropriate Standard Dilution to each standard well.
1. Add 50uL Total Glutathione Reagent or Oxidized Glutathione Reagent to each treated well, vehicle control well, and untreated control well.
1. Add 50uL Total Glutathione Reagent to each standard well.
1. Shake 5 minutes at room temperature.
1. Prepare Luciferin Generation Reagent.
1. Add 50uL Luciferin Generation Reagent to each well.
1. Shake briefly and incubate 30 minutes at room temperature.
1. Prepare Luciferin Detection Reagent.
1. Add 100uL Luciferin Detection Reagent to each well.
1. Shake briefly and equilibriate 15 minutes at room temperature.
1. Read luminescence from plate using 1 seconds per plate integration time (Promega recommends 0.25-1 second). Do not use a fluorometer and do not use filters with the luminometer.


# RECIPES

__Note__: Thaw kit reagents at room temperature (don't use the 37C water bath)

## Standard Dilutions

  * Use 5mM Glutathione (provided in kit) to make 0, 5, 10, 20, 40, 80, 160, and 320uM standard dilutions in water (see setup sheet).
  * Use Gluthathione dilutions within 30 minutes of preparation

## Total Glutathione Lysis Reagent

Per well of a 96 well plate (multiply by number of treated wells, vehicle control wells, untreated control wells, and standard wells plus 5-10% for pipette loss):
  * 1.0uL Luciferin-NT (provided in kit)
  * 10.0uL Passive Lysis Buffer 5X (provided in kit)
  * 39.0uL mqWater
  * Use within 30 minutes of preparation.

## Oxidized Glutathione Lysis Reagent

Per well of a 96 well plate (multiply by number of treated wells, vehicle control wells, and untreated control wells plus 5-10% for pipette loss):
  * 1.0uL Luciferin-NT (provided in kit)
  * 0.5uL NEM 25mM (provided in kit)
  * 10.0uL Passive Lysis Buffer 5X (provided in kit)
  * 38.5uL mqWater
  * Use within 30 minutes of preparation.

## Luciferin Generation Reagent
  * 1.25uL 100mM DTT (provided in kit)
  * 3.0uL Glutathione-S-Tranferase (provided in kit)
  * 45.75uL Glutathione Reaction Buffer (provided in kit)

## Luciferin Detection Reagent

  * Transfer the contents of one bottle of Reconstitution Buffer with Esterase to the amber bottle of lyophilized Luciferin Detection Reagent.
  * Mix by inversion until the substrate is thoroughly dissolved. Do not vortex.


[1]: https://www.promega.com/-/media/files/resources/protocols/technical-manuals/101/gsh-gssg-glo-assay-protocol.pdf?la=en
