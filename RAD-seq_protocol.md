---
layout: page
title: RAD-seq library prep
categories: protocol
---
Based on Nicolas Devos' modified version of Parchman, Gompert, Buerkle (ver. 2.3 Aug 2011) with additional modification by Blanka Shaw.

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

25 ul reaction. Prepare all on ice. Master mix in tall tube that fits 120 reactions, pipette individually into the plate wells. Prepare master mix of 120% needed volume, the enzymes are viscous and large volume is lost by adhesion to the outside of pipette tips.

In each reaction:
  * DNA + water to equal 200ng in 10uL (20ng/uL)
  * 0.5 ul EcoRI
  * 1 ul MseI
  * 2.55 ul cuttsmart buffer (comes with enzymes)
  * 11 ul dH2O

Seal the plate, vibrate plate over vortex machine, centrifuge, and incubate in PCR machine for 3 hrs at 37C, then 10min at 65C for permanent inactivation of the enzymes.

## Ligation of adaptors

### Prepare the adaptors:

Mix 1 ul of each oligo (barcoded EcoRI primers, stored in plates; melt the plates in cold water, otherwise they melt for 2 hrs on air) in a pair into 98 ul of dH2O on a plate (you cannot pipette less than 1 ul. You won’t need the whole 100 ul volume. It results in 1 uM dilutions of the adaptor. These dilutions are probably stable and can be frozen for later use

Mix 10 ul of MseI1 and MseI2 oligos (100 ul primer stock) with 80 ul H2O to make 10 uM stock (calculate final volume depending on the number of reactions). This adaptor is the same for each reaction. Sequencing only occurs from the EcoRI side, so there’s no need to barcode the MseI oligos

Incubate both mixtures for 5 min at 95C in PCR machine

Let very slowly cool in covered Styrofoam box to room temperature to obtain double-stranded adaptor stock

### Perform the ligation:

12 ul reaction (once again, prepare mastermix of 120% needed volume, the enzymes are viscous and large volume is lost by adhesion to the outside of pipette tips).

In each reaction:
  * 9 ul of digested DNA
  * 1 ul of EcoRI adaptors (contain barcodes, NOT in master mix!)
  * 2uL Master Mix:
    * 0.2 ul of T4 DNA ligase
    * 1 ul of MseI adaptor
    * 0.12 ul ligase 10x buffer
    * 0.7 ul dH2O

Seal the plate, vibrate plate over vortex, centrifuge, and incubate in PCR machine for 1 hrs at 23C.

## PCR on ligated fragments

Prepare a mastermix of 120% needed volume (or optionally, two master mixes for two plates to reduce stochastic pcr variations):

In each reaction:
  * 2uL ligated DNA
  * 18uL Master Mix:
    * 8 ul H2O
    * 4 ul 5x buffer
    * 4 ul dNTPs
    * 0.4 ul MgCl2
    * 1.3 ul primer mix (primer1 + primer2)
    * 0.2 ul Taq (iProof)
    * 0.15 ul DMSO

20 ul reaction, in PCR machine: 98C for 30 sec, 30 cycles of: 98C for 20sec, 60C for 30sec, 72C for 40sec, final extension at 72C for 10 min.

If two plates, pool the two PCR products for each sample into one.

Quantify the DNA with Qubit.

## Pooling equal concentrations of each sample DNA

We want 100 ng of DNA per sample. Pool volume corresponding to 100 ng from each well (usually 3-7ul). Lower concentration PCR products can be attempted at risk of reduced reads.

## Fragment size selection

AMP beads are used to keep fragments of 350 bp long, see the protocol for library prep from Illumina.

2 steps: remove larger fragments with diluted beads, then remove small fragments with undiluted beads; it works by changing the ratio of the beads to DNA. For convenience, add water to the pooled sample to have 500 ul total volume of pooled DNAs for size selection (or equivalent of whole 100).

Beads need to be in room temperature, and be vortexed all the time, they settle fast.

### Step1

Divide your pooled DNA library into 100 ul batches in 1.5ml Eppendorf tubes (you’ll have 4-5).

For 350 bp insert size selection, prepare diluted beads solution: 109.25 ul beads + 74.75 ul DEPC water for each 100ul tube (546.25 ul beads + 375.75 ul H2O for 5 tubes). Vortex solution for 5 sec to distribute evenly.

Add 160 ul of diluted beads into each 100 ul sample tube. Pipette up and down 10 times or more to mix well.

Incubate 5 min at room temperature for beads to bind large fragments.

Meanwhile, prepare fresh 80% ethanol in 100 ml cylinder (84.2 ml of 190proof ethanol, fill DEPC water to 100 ml).

Put tubes into the magnetic stand – beads start to accumulate and the liquid is clearing, 5 min. Collect the liquid = transfer 2 x 125 ul of the supernatant without disturbing the beads. Discard tubes with beads and remaining diluted beads.

### Step 2

Vortex beads again for 1 min or until completely dispersed. Add 30 ul of undiluted beads into each tube (containing 250 ul of supernatant). Pipette up and down, and incubate for 5 min away from magnets.

Place tubes on magnetic stand for 5 min. Then carefully remove 138 ul of supernatant, twice, without disturbing the beads (if little left, it’s fine, it gets washed). This time the DNA is on the beads.

Keep the tubes on the magnetic stand. Add 200 ul of 80% ethanol in each tube without disturbing the beads. Incubate 30 sec, then remove. Repeat second time. Remove traces of ethanol with 10 ul pipette. Let the beads dry for about 5 min. Beads should not be shiny (wet) but they also should not crack.

Add 20 ul of DEPC water (or resuspension buffer) to each well, run it over the beads but don’t touch them. Pipette over the beads until they resuspend, and pipette up and down 10 times to mix well. Incubate for 2 min at room temp.

Place tubes on magnetic stand for 5 min. Then carefully transfer 17.5 ul of clear supernatant to labeled tube.

Measure concentration on Qubit.

Submit for sequencing. The sequencing center will use qPCR/bioanalyzer to determine if additional size selection or cleaning is necessary and process as needed. It may require additional gel cut for better size selection. However, size selecting on gel without the bead cleaning seem to not be sufficient.

# Recipes
