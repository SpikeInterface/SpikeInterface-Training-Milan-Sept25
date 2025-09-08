# SpikeInterface-Training-Milan-Sept25

Material for SpikeInterface Tutorial @ Human Technopole - Milan - September 2025


## Schedule

**Day 3 - Session 1 (2h) - Wed 24/09 11:00-13:00**

1. 45-60min: Introduction to Spike Sorting (detailed theoretical) - Sam
2. 30-45min: Introductionto to SpikeInterface - Alessio
3. 15-30min: Installation check, get jupyter lab ready to go (trivial test notebook to run) - Chris


**Day 3 - Session 2 (3h) - Wed 24/09 14:00-17:00**
Step-by-step hands-on tutorial

1. Reading  + Manipulation (30 min - Chris)
Read data + visualize + select_channels+time_slice (DEMO + HAND-ON)
Attach probe (on 32ch simulated recording): create a 4-shank probe with 8 channels and attach it to the simulated recording (DEMO)
Save to JSON

2. Preprocess (DEMO - point to docs - skip remove artifacts + save recording - job_kwargs) (45 min) (Alessio)
HAND-ON: apply+visualize preprocessing 
HAND-ON: check if there are bad channels and see if detect bad channels finds them all?
(DEMO) Drift: only estimation + plotting for quality control (Sam)

3. Spike sort (DEMO - Kilosort4 - maybe ok on CPU) (30 min) (Sam)
HAND-ON: run SpykingCIRCUS2 - are there differences? #units / #spikes 
(optional: comparison)
Comparison - plot agreements (DEMO)

4. Analyze Sorting (DEMO + HAND-ON) (45 min) (Chris)
Create analyzer and compute extensions (DEMO)
Hands-on 1: get the SNR distribution and plot an histogram
Hands-on 2: plot ACG of best/worst SNR unit
Hands-on 3: use the SI API to get extremum channels/amplitudes etc and plot the template in matplotlib

5. Curate (30 min) (Alessio) 
Threshold-based
Model-based
merge
(Manual: SIGUI - teaser for next day)

**Day 4 - Session 3 (3.5h) - Thu 25/09 09:30-13:00**

1. 1hr: SpikeInterface-GUI - (DEMO + HANDS ON) (Sam)

2. 2.5hr: DEVELOP A FULL PIPELINE SCRIPT (Chris)




## Installation




## Dataset
