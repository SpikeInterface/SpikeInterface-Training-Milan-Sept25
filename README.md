# SpikeInterface-Training-Milan-Sept25

Material for SpikeInterface Tutorial @ Human Technopole - Milan - September 2025


## Schedule

**Day 3 - Session 1 (2h) - Wed 24/09 14:00-15:00**

1. 30min: Introduction to Spike Sorting (detailed theoretical) - Sam
2. 25min: Introductionto to SpikeInterface - Alessio
3. 5min: Installation check, get jupyter lab ready to go (trivial test notebook to run) - Chris


**Day 3 - Session 2 (3h) - Wed 24/09 15:00-18:00**


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
HAND-ON: run tridesclous2 - are there differences? #units / #spikes 
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

We recommend that you [install uv](https://docs.astral.sh/uv/getting-started/installation/). This is an unbelievably good new package
management tool for Python.

Open your Terminal app and cd (change directory) to where you like to keep github repos. Then clone this repo, and navigate to the `notebooks` folder of it by entering the following commands into your Terminal:

``` shell
git clone https://github.com/SpikeInterface/SpikeInterface-Training-Milan-Sept25.git
cd SpikeInterface-Training-Milan-Sept25/notebooks/
```

Now open jupyter lab (you don't need to install this - uv will take care of it) using uv:

``` shell
uv run jupyter lab
```

Or if you prefer to use vscode:

``` shell
uv run code .
```

If you like traditional virtual environments, please visit [this page](https://github.com/SpikeInterface/spikeinterface/tree/main/installation_tips) to install on your laptop python+spikeinterface.

Computing node with a preinstalled environement will be also provided.

## Dataset

Please download theses datasets on your laptop:
1. 4-tetrodes recording : ...
2. Nueopixels2.0 one-shank 20min  : ...
3. In vitro recording : ...
