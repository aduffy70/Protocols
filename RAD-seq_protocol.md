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

Extract DNA and quantify with Qubit. Concentrations should be at least 20ng/uL (though lower concentrations can be attempted)

## Digestion

25 ul reaction. Prepare all on ice. Master mix in 2mL tube that fits 120 reactions, pipette individually into the plate wells. Prepare master mix of 120% needed volume, the enzymes are viscous and large volume is lost by adhesion to the outside of pipette tips.

In each reaction:
  * DNA + water to equal 200ng in 10 uL (20ng/uL)
  * 15 uL Digestion Master Mix

Seal the plate, vibrate plate over vortex machine, centrifuge, and incubate in PCR machine for 3 hrs at 37C, then 10min at 65C for permanent inactivation of the enzymes.

## Ligation of adaptors

### Prepare the adaptors (if needed--we prepare enough for several libraries at a time):

Mix 1 ul of each oligo (barcoded EcoRI primers, stored in plates; melt the plates in cold water, otherwise they melt for 2 hrs on air) in a pair into 98 ul of dH2O on a plate (you cannot pipette less than 1 ul. You won’t need the whole 100 ul volume. It results in 1 uM dilutions of the adaptor. These dilutions are probably stable and can be frozen for later use

In small pcr tubes, mix 14 ul of 100uM MseI1 oligo and 14 uL of 100uM MseI2 oligo with 112 ul H2O to make 10 uM stock. This makes 140uL per tube and we need 120uL for a 96 sample library. This adaptor is the same for each reaction. Sequencing only occurs from the EcoRI side, so there’s no need to barcode the MseI oligos

Incubate both mixtures for 5 min at 95C in PCR machine

Let very slowly cool in covered Styrofoam box to room temperature to obtain double-stranded adaptor stock

### Perform the ligation:

12 ul reaction (once again, prepare master mix of 120% needed volume in a 1.5mL tube, the enzymes are viscous and large volume is lost by adhesion to the outside of pipette tips).

In each reaction:
  * 9 ul of digested DNA (multipipetter works for this)
  * 1 ul of EcoRI adaptors (contain barcodes, NOT in master mix! Multipipetter works. Reseal plate with a NEW seal (labelled with number of times thawed) or they will evaporate in the freezer!)
  * 2 uL Ligation Master Mix


Seal the plate, vibrate plate over vortex, centrifuge, and incubate in PCR machine for 1 hrs at 23C.

Dilute each reaction with 88uL water. Store at 4C for a month or -20C for longer.

## PCR on ligated fragments

Prepare a master mix of 120% needed volume in a 5mL tube (or optionally, two master mixes for two plates to reduce stochastic pcr variations):

In each reaction:
  * 18uL PCR Master Mix
  * 2uL ligated DNA (multipipetter works)


20 ul reaction, in PCR machine: 98C for 30 sec, 30 cycles of: 98C for 20sec, 60C for 30sec, 72C for 40sec, final extension at 72C for 10 min.

If two plates, pool the two PCR products for each sample into one.

Quantify the DNA with Qubit. Recent results average ~12.5ng/uL

## Pooling equal concentrations of each sample DNA

Take AMP beads and DEPC water out of the fridge now so they have hours to warm to room temperature for the fragment size selection step. Let them warm while pooling samples.  

We want 100 ng of DNA per sample. Pool volume corresponding to 100 ng from each well (usually ~8uL) into a 1.5mL tube. Lower concentration PCR products can be attempted at risk of reduced reads.

## Fragment size selection

AMP beads are used to keep fragments of 350 bp long, see the protocol for library prep from Illumina.

2 steps: remove larger fragments with diluted beads, then remove small fragments with undiluted beads; it works by changing the ratio of the beads to DNA. For convenience, add water to the pooled sample to have 700 ul total volume of pooled DNAs for size selection (or equivalent of whole 100).

Beads need to be in room temperature, and be vortexed all the time, they settle fast.

### Step1

Divide your pooled DNA library into 100 ul batches in 1.5ml Eppendorf tubes (you’ll have ~7).

For 350 bp insert size selection, prepare diluted beads solution: 109.25 ul beads + 74.75 ul DEPC water for each 100ul tube (546.25 ul beads + 375.75 ul H2O for 5 tubes). Vortex solution for 5 sec to distribute evenly.

Add 160 ul of diluted beads into each 100 ul sample tube. Pipette up and down 10 times or more to mix well.

Incubate 5 min at room temperature for beads to bind large fragments.

Meanwhile, prepare fresh 80% ethanol in 50 ml cylinder (21 ml of 190proof ethanol, fill DEPC water to 25 ml).

Put tubes into the magnetic stand – beads start to accumulate and the liquid is clearing, 5 min. Collect the liquid = transfer 2 x 125 ul of the supernatant without disturbing the beads. Discard tubes with beads and remaining diluted beads.

### Step 2

Vortex beads again for 1 min or until completely dispersed. Add 30 ul of undiluted beads into each tube (containing 250 ul of supernatant). Pipette up and down, and incubate for 5 min away from magnets.

Place tubes on magnetic stand for 5 min. Then carefully remove 138 ul of supernatant, twice, without disturbing the beads (if little left, it’s fine, it gets washed). This time the DNA is on the beads.

Keep the tubes on the magnetic stand. Add 200 ul of 80% ethanol in each tube without disturbing the beads. Incubate 30 sec, then remove. Repeat second time. Remove traces of ethanol with 10 ul pipette. Let the beads dry for about 5 min. Beads should not be shiny (wet) but they also should not crack.

Still on the magnets, add 20 ul of DEPC water (or resuspension buffer) to each well, run it over the beads but don’t touch them. Pipette over the beads until they resuspend, then remove from the magnet and pipette up and down 10 times to mix well. Incubate away from the magnets for 2 min at room temp.

Place tubes on magnetic stand for 5 min. Then carefully transfer 17.5 ul of clear supernatant to labeled tube.

Measure concentration on Qubit. 3--5ng/uL is typical.

Submit for sequencing. The sequencing center will use qPCR/bioanalyzer to determine if additional size selection or cleaning is necessary and process as needed. It may require additional gel cut for better size selection. However, size selecting on gel without the bead cleaning seem to not be sufficient.

# Recipes

## Digestion master mix

|     |    | Per rxn | 48 rxns (+20% = 60) | 96 rxns (+20% = 120) |
| --- | -- | ------- | ------------------- | -------------------- |
|dH2O	| ul | 11 | 660 | 1320 |
|cutsmart buffer | ul | 2.5 | 150 | 300 |
|MseI enzyme | ul | 1 | 60 | 120 |
|EcoRi enzyme | ul | 0.5 | 30 | 60 |

## Ligation master mix

|     |    | Per rxn | 48 rxns (+20% = 60) | 96 rxns (+20% = 120) |
| --- | -- | ------- | ------------------- | -------------------- |
| dH2O | ul | 0.7 | 42 | 84 |
| ligase 10x buffer | ul | 0.12 | 7.2 | 14.4 |
| MseI adaptor | ul | 1 | 60 | 120 |
| T4 ligase enzyme | ul | 0.2 | 12 | 24 |

## PCR master mix

|     |    | Per rxn | 48 rxns (+20% = 60) | 96 rxns (+20% = 120) |
| --- | -- | ------- | ------------------- | -------------------- |
| dH2O | ul | 8 | 480 | 960 |
| 5x buffer | ul | 4 | 240 | 480 |
| 1mM dNTPs | ul | 4 | 240 | 480 |
| MgCl2 | ul | 0.4 | 24 | 48 |
| Ill PCR 1+2 premix | ul | 1.3 | 79.8 | 159.6 |
| DMSO | ul | 0.15 | 9 | 18 |
| iProof Taq | ul | 0.2 | 12 | 24 |

Note: PCR premix is 9uL of 100uM primer1 + 9uL of 100uM primer2 + 162uL water (5uM each primer or 10uM primer total)
