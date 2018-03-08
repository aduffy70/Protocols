---
layout: page
title: Epoxide trapping assay
categories: protocol
---

Adapted from existing Coulombe Lab protocols

# Assay:

1. Prepare setup sheet.
1. Thaw (or prepare) cofactor stocks and buffer at room temperature. Start water bath (37C).
1. Thaw microsomes (yellowish) and cytosol (pinkish) on ice.
1. Thaw AFB in the dark at room temperature (200ul aliquot).
1. Make dilutions of AFB, microsomes, and cytosol.
1. Make cofactor mix on ice.
1. Put buffer into rxn tubes on ice.
1. Add cytosol and microsomes and mix.
1. Start timer, add cofactor at 0 and every 60 seconds, mix, place on ice.
1. Add AFB at 10min, mix and put in water bath.
1. Prepare stopping solution
  * Take A365 reading blanked with MeOH (expected reading = 0.09)
  * A365 reading / 0.0225 = uM AFG (expected = 4uM)
1. At 30min, add 250ul AFG mix, place on ice.
1. Store tubes at -20C overnight.

# HPLC:

## Setup

1. Fill C (HPLC MeOH), D (HPLC water), and wash (HPLC MeOH) bottles.
1. Change guard column, if needed.
1. Turn on components in counter clockwise order (pump, sampler, oven, detector, controller).
1. Unplug internet line and turn on computer.
1. Start LC Solution, 1 - real time analysis (no pswd).
1. Open data acquisition from left (click top arrow if necessary).
1. Click on methods tab.
1. Open start up method.
1. Set instrument parameters to 50%C, 50%D and download.
1. Open purge valve. Turn on pump and oven (via icon).
1. Run ~5 minutes at 2ml/min then ~5-15 minutes at 1ml/min to remove air from lines. Close valve (if oven is 40C).
1. Let run 15 min, making sure pressure is stable. Note pressure (~1750).
1. Make buffer A.
1. Open valve and purge with 0%B.
1. Make buffer B.
1. Purge with 100%B.
1. Purge at 50% B and close valve.
1. Run at 1ml/min until stable. Note pressure (~1750).
1. Run at 10% B. Note pressure (~1250).
1. Lower to .5ml/min until ready to start run.
1. Set up batch table.
1. Change data file names (date and sample #).
1. Spin samples (13.2rpm, 11min), filter and load into sampler with 50% HPLC MeOH:HPLC water blank.
1. Start run.

## Collect and process standard

1. When the standard sample is injected (about 45 minutes after run starts), collect the AFB-gsh peak (~16.5 -16.8 minutes into the standard sample). Start collecting at top of peak and collect for 2 minutes.
1. Take A365 reading of AFB-gsh blanked with 30% HPLC MeOH:HPLC water.
1. Make 24.4uM AFG from 122uM stock:
  * 100uL 122uM AFG
  * 400uL HPLC MeOH
1. Take A365 reading of 24.4uM AFG blanked with MeOH. Expected reading = 0.549.
1. Make standard dilutions according to table, make 2 aliquots of 165uL per standard sample (S1-S5 and S1a-S5a) in HPLC vials, and load vials into sampler:

| Sample | AFB-gsh uL | 30% HPLC MeOH uL | 24.4uM AFG uL |
| ------ | ---------- | ---------------- | ------------- |
| S1 | 350 (175 + 175) | 0 | 14 |
| S2 | 175 | 175 | 14 |
| S3 | 87.6 | 262.4 | 14 |
| S4 | 43.8 | 306.2 (153.0 + 153.2) | 14 |
| S5 | 21.9 | 328.2 (164.0 + 164.2) | 14 |


## Post-run

1. Next day, stop batch.
1. Switch to clean guard column.
1. Run clean and store batch.
1. Close program.
1. Turn off components in same order.
1. Close up waste container.
1. Find data and shift or control click on runs. Right click, file conversion to ASCII. Output items, file properties and peak table. Save to the desired drive.
1. Import data to Setup/analysis sheet.

# RECIPES

## Trapping Buffer (80mM Potassium Phosphate, 25mM KCl, 5mM MgCl2, 0.25mM sucrose, pH 7.6):

200x Sucrose (0.05M):
  * 0.21g sucrose (342.3 mw)
  * water to 12mL
  * Make 1.1 and 0.6ml aliquots, store at -20.

200x MgCl2-6H2O (1.23M):
  * 2.5g MgCl2-6H2O (203.31 mw)
  * water to 10mL
  * Make 1.1 and 0.6ml aliquots, store at -20.

100x KCl (2.5M):
  * 5g KCl (74.55 mw)
  * water to 27mL
  * Make 1.1ml aliquots, store at -20.

10x K2HPO4 (0.8M):
  * 7g K2HPO4 dibasic (174.18 mw)
  * water to 50mL
  * Store in fridge

10x KH2PO4 (0.8M):
  * 5.4g KH2PO4 monobasic (136.09 mw)
  * water to 50mL
  * Store in fridge

Buffer 1 (80mM K2HPO4 dibasic, pH~8.8):
  * 10mL 10X K2HPO4
  * 90mL water

Buffer 2 (80mM KH2PO4 monobasic, “low” pH):
  * 10mL 10X KH2PO4
  * 0.5ml 200x sucrose
  * 0.5ml 200x MgCl
  * 1ml 100x KCl
  * water to 100mL
  * store in fridge

Trapping buffer
  * 100mL Buffer 1
  * Add ~10ml Buffer 2 to bring pH ~7.8. (So precipitates do not form in next steps)
  * Then add:
    * 0.5ml 200x sucrose
    * 0.5ml 200x MgCl
    * 1ml 100x KCl
  * Add ~4.5ml Buffer 2 to bring final pH to 7.6

## 10X Cofactor Mix (20mM NADPH, 50mM GSH)

NADPH (0.2M):
  * 0.1g NADPH (Sigma N1630, 833.35 mw)
  * 0.5mL Trapping buffer
  * Make 110ul aliquots, store at -20.

GSH (Sigma G6529, 0.2M):
  * 0.1g GSH (307.32mw)
  * 1.5mL Trapping buffer
  * Make 260ul aliquots, store at -20.

10X Cofactor Mix:
  * 100uL NADPH
  * 250uL GSH
  * 650uL Trapping buffer

## AFB Substrate (32mM):
  * 10 mg AFB (Sigma A6636, 312.27 mw)
  * 1mL DMSO
  * Make 200ul aliquots, wrap in foil and store -20.

## AFG Internal Standard (122uM AFG in HPLC MeOH):

30.5mM AFG:
  * 10mg AFG (A0138, 328.27mw)
  * 1ml DMSO

AFG Internal Standard:
  * 40uL 30.5mM AFG
  * 9.96mL HPLC MeOH
  * Make 1.5mL aliquots, store at -20.

## Stopping solution:
  * 520uL 122uM AFG
  * 15.08mL ice cold HPLC MeOH

## HPLC Buffer A (Need 30mL/run + 300mL)

For 2L:
  * 3.74g monobasic KH<sub>2</sub>PO<sub>4</sub>
  * 1.44mL H<sub>3</sub>PO<sub>4</sub>
  * HPLC water to 2L

## HPLC Buffer B (Need 15mL/run + 200mL)

For 1L:
  * 50mL THF
  * 950mL HPLC MeOH
