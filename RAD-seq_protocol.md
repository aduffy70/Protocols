---
layout: page
title: RAD-seq library prep
categories: protocol
---
Based on Nicolas Devos' modified version of Parchman, Gompert, Buerkle (ver. 2.3 Aug 2011) with additional modification by Blanka Aguero.

# Process

1. DNA extraction and quantification
1. Digestion (EcoRI, MseI)
1. Ligation (EcoRI adaptors with barcodes, MseI adaptors)
1. PCR on ligated fragments and quantify PCR products
1. Pooling equal concentrations of each sample DNA
1. Fragment size selection of pooled library using AMP beads
1. Quantify size-selected library and submit for sequencing

## DNA extraction and quantification

Extract DNA and quantify with Qubit HS reagents using 2uL sample. Concentrations should be at least 20ng/uL (though lower concentrations can be attempted).

## Digestion

25uL reaction. Prepare all on ice. Master mix in 2mL tube that fits 110 reactions, pipette individually into the plate wells. Prepare master mix of 115% needed volume, the enzymes are viscous and large volume is lost by adhesion to the outside of pipette tips.

In each reaction:
  * DNA + water to equal 200ng in 10uL (20ng/uL)
  * 15uL Digestion Master Mix

Digestion master mix:

|     |    | Per rxn | 96 rxns (+15% = 110) |
| --- | -- | ------- | -------------------- |
|dH2O	| uL | 11 | 1210 |
|cutsmart buffer | uL | 2.5 | 275 |
|MseI enzyme | uL | 1 | 110 |
|EcoRi enzyme | uL | 0.5 | 55 |

Seal the plate, vibrate plate over vortex machine, centrifuge, and incubate in PCR machine for 3 hrs at 37C, then 10min at 65C for permanent inactivation of the enzymes.

## Ligation of adaptors

### Prepare the adaptors (if needed--we prepare enough for several libraries at a time):

Mix 1uL of each oligo (barcoded EcoRI primers, stored in plates; melt the plates in cold water, otherwise they melt for 2 hrs on air) in a pair into 98uL of dH2O on a plate (you cannot pipette less than 1uL. You won’t need the whole 100uL volume. It results in 1 uM dilutions of the adaptor. These dilutions are stable and can be frozen for later use.

In small pcr tubes, mix 14uL of 100uM MseI1 oligo and 14uL of 100uM MseI2 oligo with 112uL H2O to make 10uM stock. This makes 140uL per tube and we need 120uL for a 96 sample library. This adaptor is the same for each reaction. Sequencing only occurs from the EcoRI side, so there’s no need to barcode the MseI oligos.

Incubate both mixtures for 5 min at 95C in PCR machine.

Let very slowly cool in covered Styrofoam box to room temperature to obtain double-stranded adaptor stock.

### Perform the ligation:

12uL reaction (prepare master mix of 120% needed volume in a 1.5mL tube, the enzymes are viscous and large volume is lost by adhesion to the outside of pipette tips).

In each reaction:
  * 9uL of digested DNA (multipipetter works for this)
  * 1uL of EcoRI adaptors (contain barcodes, NOT in master mix! Multipipetter works. Reseal plate with a NEW seal (labeled with number of times thawed) or they will evaporate in the freezer!)
  * 2uL Ligation Master Mix

Ligation master mix:

|     |    | Per rxn | 96 rxns (+20% = 120) |
| --- | -- | ------- | -------------------- |
| dH2O | uL | 0.7 | 84 |
| ligase 10x buffer | uL | 0.12 | 14.4 |
| MseI adaptor | uL | 1 | 120 |
| T4 ligase enzyme | uL | 0.2 | 24 |


Seal the plate, vibrate plate over vortex, centrifuge, and incubate in PCR machine for 1 hr at 23C, then 10min at 65C for permanent inactivation of the enzymes.

Dilute each reaction with 88uL water. Store at 4C for a month or -20C for longer.

## PCR on ligated fragments

Prepare a master mix of 115% needed volume in a 2mL tube:

In each reaction:
  * 14uL PCR Master Mix
  * 6uL ligated DNA (multipipetter works)

PCR master mix:

|     |    | Per rxn | 96 rxns (+15% = 110) |
| --- | -- | ------- | -------------------- |
| dH2O | uL | 4 | 440 |
| 5x buffer | uL | 4 | 440 |
| 1mM dNTPs | uL | 4 | 440 |
| MgCl2 | uL | 0.4 | 44 |
| Ill PCR 1+2 premix | uL | 1.2 | 132 |
| DMSO | uL | 0.2 | 22 |
| iProof Taq | uL | 0.2 | 22 |

Note: PCR premix is 9uL of 100uM primer1 + 9uL of 100uM primer2 + 162uL water (5uM each primer or 10uM primer total)

20uL reaction, in PCR machine: 98C for 30 sec, 30 cycles of: 98C for 20sec, 60C for 30sec, 72C for 40sec, final extension at 72C for 10 min.

Quantify the DNA with Qubit HS reagents using 2uL sample. Recent results average ~12.5ng/uL.

## Pooling equal concentrations of each sample DNA

Take AMPure beads and DEPC water out of the fridge now so they have hours to warm to room temperature for the fragment size selection step. Let them warm while pooling samples.  

We want to pool an equal amount of DNA per sample. Select an amount that 1) can be met for all (good*) samples using <=18uL (the amount we have left after Qubit), and 2) will yield 1250-1300uL total pool size so we can size-select and clean in 6 batches of 200uL (allowing for pipetting loss). Typical amounts are 150ng-200ng per sample. Calculate the needed volume for each sample and pool into a 1.5mL tube.

*Lower concentration PCR products can be attempted at risk of reduced reads.

## Fragment size selection

AMPure beads in a PEG/salt solution are used to select mid-sized fragments approximately 350 bp long in three steps:
1) Bind larger DNA fragments to the beads with a 0.6X diluted concentration of PEG/salt and keep the solution containing the small and mid-sized DNA fragments.
2) Add more AMPure beads stock solution to increase the PEG/salt concentration to 0.8X to bind mid-sized DNA fragments to the beads and discard the solution containing small DNA fragments.
3) Wash the mid-sized fragments on the beads with 80% EtOH and then elute in a small quantity of DEPC water to get a clean and concentrated final library.

Beads need to be at room temperature and to be vortexed all the time, they settle fast.

### Step 1

Divide the pooled DNA library into 200uL batches in six 1.5mL Eppendorf tubes. Discard any extra or add water to make sure each batch is exactly 200uL.

Place the six tubes on the magnetic stand away from the magnets.

Vortex AMPure beads stock solution for 1 min to mix thoroughly.

In a 2mL tube, prepare enough diluted beads solution for the 6 batches:

|     |    | Per batch (+5% extra) | 6 batches (+5% extra) |
| --- | -- | ------- | -------------------- |
| AMPure beads stock solution | uL | 200 | 1200 |
| dH2O | uL | 136 | 816 |

Vortex diluted beads solution for 5-10s to mix thoroughly.

Add 320 uL of diluted beads solution into each 200 uL sample. Pipette up and down 10 times or more to mix well. Discard any excess diluted beads solution.

Incubate tubes for 5 min AWAY FROM from the magnets.

Meanwhile, prepare fresh 80% ethanol in a 15mL falcon tube: 10.5mL 190proof EtOH + 2000uL DEPC water (room temperature).

__Important-__ EtOH and water are miscible so to get the correct concentration they must be measured separately and then mixed. Don't measure by putting 10.5mL EtOH in a tube and then adding water to a final concentration of 12.5mL. The concentration will be wrong!

Incubate tubes for 5 min ON the magnets to accumulate the beads and clear the liquid.

Without disturbing the beads, collect 500uL of the liquid from each tube and transfer to a new set of six 1.5mL tubes. Use a 200uL pipette to avoid disturbing the beads (4 X 125uL = 500uL). Pipette slowly so liquid has time to settle to the bottom of the tube as you go. Discard the tubes with beads.

### Step 2

Vortex AMPure bead stock solution again for 1 min.

Add 60uL of undiluted AMPure beads stock solution into each 500uL sample. Pipette up and down 10 times or more to mix well.

Incubate tubes for 5 min AWAY FROM the magnets.

Incubate tubes for 5 min ON the magnets to accumuLate the beads and clear the liquid.

Without disturbing the beads, remove and discard the liquid. Use a 200uL pipette to avoid disturbing the beads (3 X 184uL). It is ok if a small amount of liquid remains--it will get cleaned.

Keep the tubes with the beads (and our DNA) ON the magnets.

### Step 3

With the tubes still ON the magnets, add 400uL of 80% EtOH to each tube without disturbing the beads.

Incubate 30 sec ON the magnets to wash.

Without disturbing the beads, remove the EtOH with a 200uL pipetter (2 X 200uL).

Repeat to wash a second time with 400uL 80% EtOH.

With the tubes still ON the magnets, remove traces of ethanol with a 10uL pipette.

Let the beads dry for 5 min. Beads should not be shiny (wet) but they also should not crack.

With the tubes still ON the magnets, Add 30uL of DEPC water to each tube (2 X 15uL with a 20uL pipette). Run the water over the beads but don’t touch them. Pipette over the beads until they resuspend, then remove the tube from the magnet and pipette up and down 10 times to mix well.

Incubate tubes 2 min AWAY FROM the magnets.

Incubate tubes 5 min ON the magnets to accumulate the beads and clear the liquid.

Without disturbing the beads, transfer 28uL of the liquid from each tube to a single new 1.5mL tube (2 X 14uL with a 20uL pipetter). This is the finished library with a total volume of approximately 168uL.

## Quantify library and submit for sequencing

Measure concentration on Qubit with HS reagents. Use 10uL of the library to make the measurement to get a more accurate measurement at the expected small concentrations. 3--7ng/uL is typical.

Submit for sequencing. The sequencing center will use qPCR/bioanalyzer to determine if additional size selection or cleaning is necessary and process as needed.

# Recipes
