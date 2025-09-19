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


# Overview of available datasets

## In vivo

### M25_D23_2024-11-11_13-11-10_OF1

Neuropixels 2.0 dataset (384 channels) acquired with the Open Ephys GUI in binary format.
You can use the `spikeinterface.extractor.read_openephys()` function to read the data.

### 1544_2023-04-21_09-55-34_of

Recording with 16 channels organized in 4 tetrodes acquired with the Open Ephys GUI in "openephys" format.
You can use the `spikeinterface.extractor.read_openephys()` function to read the data.

### aind_ecephys_session.zarr

Recording with a Neuropixels 2.0 - 4 shank probe stored as a compressed SpikeInterface Zarr folder.
You can use the `spikeinterface.load()` (or `spikeinterface.read_zarr()`) function to read the data.

### cambridgeNT_openephys

Recording with a Cambridge Neurotech [ASSY-236-H5](https://github.com/SpikeInterface/probeinterface_library/blob/main/cambridgeneurotech/ASSY-236-H5/ASSY-236-H5.png) probe and wired to the Open Ephys acquisition system via the 
Cambridge NeuroTech mini-amp-64.
You can use the `spikeinterface.extractor.read_openephys()` function to read the data.
The probe is available from the [probeinterface_library](https://github.com/SpikeInterface/probeinterface_library) (see [docs](https://probeinterface.readthedocs.io/en/main/examples/ex_10_get_probe_from_library.html) here) and the wiring is available in [`ProbeInterface`](https://probeinterface.readthedocs.io/en/main/examples/ex_11_automatic_wiring.html#).


## In vitro

### mouse_CTX_14D.brw

Primary mouse cortex for E18 embryos. Plated 80K on CorePlate 1W38/60 3Brain, recorded after 14 days in culture 
with 3Brain BioCAM system. 
You can use the `spikeinterface.extractor.read_biocam()` function to read the data. 


### human_ngn2_100K_c_55D.brw

Human glutamatergic neurons induced via ngn2 method. Plated 100k on CorePlate 1W38/60 3Brain, recorded after 55 days in 
culture with 3Brain BioCAM system. 
You can use the `spikeinterface.extractor.read_biocam()` function to read the data. 

> [!IMPORTANT]  
> The 3Brain BioCAM system saves the data in unsigned integers. You should convert it to signed integers for a smooth
> processing. See documentation [here](https://spikeinterface.readthedocs.io/en/latest/how_to/unsigned_to_signed.html). Note that the `bit_depth` for this system is 12!


Please download these datasets on your laptop from this link:

https://filesender.renater.fr/?s=download&token=420bcfb8-f134-473a-be40-c28235dda5da
