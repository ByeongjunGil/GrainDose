# GrainDose

Reference analysis code for the manuscript:

> **Cryogenic Cooling Accelerates Electron-Beam Damage in FAPbI<sub>3</sub>**

This repository contains the nanobeam-diffraction analysis workflow used to quantify temperature-dependent electron-beam damage in FAPbI<sub>3</sub>.

## Files

- `reference.ipynb`: complete reference analysis notebook
- `requirements.txt`: required Python packages

## Installation

```bash
git clone https://github.com/ByeongjunGil/GrainDose.git
cd GrainDose
pip install -r requirements.txt
```

## Usage

Open `reference.ipynb` and specify the input and output locations in the configuration cell:

```python
DATA_DIR = pathlib.Path("path/to/dm4/dataset/Hour_00")
OUTPUT_DIR = pathlib.Path("analysis_output")
DATASET_ID = "example_dataset"
```

The current loading cell searches for DM4 files matching:

```text
Minute_*/Second_*/*.dm4
```

If the directory structure differs, modify the file-search pattern while preserving the chronological frame order.

Run all notebook cells in order. The repository contains analysis code only and does not include the experimental datasets.

## Citation

If you use this workflow, please cite:

> Byeongjun Gil, Myung-Geun Han, Yimei Zhu, Ray Egerton, and Miyoung Kim,  
> “Cryogenic Cooling Accelerates Electron-Beam Damage in FAPbI<sub>3</sub>.”

Journal and DOI information will be added after publication.
