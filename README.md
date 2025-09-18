# SpikeInterface-Training-Milan-Sept25

Material for SpikeInterface Tutorial @ Human Technopole - Milan - September 2025


## Schedule

**Day 3 - Theoretical overview - Wed 24/09 14:00-15:00**

1. Introduction to Spike Sorting (30 min - Sam)
2. Introduction to `SpikeInterface` (25 min - Alessio)
3. Installation check, get jupyter lab ready to go (5 min - Chris)

**Day 3 - Hands on tutorials - Wed 24/09 15:00-18:00**

1. Reading + Manipulation (30 min - Chris)
    - Read and visualise data
    - The importance of probes

2. Preprocessing (45 min - Alessio)
    - Apply and visualize preprocessing 
    - Detect bad channels
    - Motion correction

3. Spike sort (30 min - Sam)
    - Run a spike sorter
    - Compare spike sorter outputs

4. Analyze Sorting (45 min - Chris)
    - Create a `SortingAnalyzer` to explore your sorting
    - Compute some extensions
    - Play with the extension outputs

5. Curate (30 min - Alessio) 
    - Simple, threshold-based curation
    - Curation using ML models
    - Merging units

**Day 4 - GUI and Pipelines - Thu 25/09 09:30-13:00**

1. SpikeInterface-GUI (60min - Sam)

*10:30-11.00: Coffee break*

2. Develop a full pipeline script (90min - Chris)
    - Basics of pipelines in Python
    - Designing a pipeline for your own data


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

Computing node with a preinstalled environment will be also provided.


## Dataset

Please download theses datasets on your laptop:

https://filesender.renater.fr/?s=download&token=420bcfb8-f134-473a-be40-c28235dda5da

1. 4-tetrodes recording : 1544_2023-04-21_09-55-34_of.zip
2. Nueopixels2.0 one-shank 20min  : M25_D23_2024-11-11_13-11-10_OF1.zip
3. In vitro recording : mouse_CTX_14D.brw

And all of then if you want.
