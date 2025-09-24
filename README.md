# MARS-HPC: Multi-objective Resilience-Aware Scheduling

MARS-HPC is a framework for **multi-objective HPC resource scheduling** using deep reinforcement learning.  
It integrates a **multi-headed DQN** with **Pareto-archive replay** to optimize energy, performance, and resilience trade-offs.  

## Features
- Multi-objective scheduling with weighted DQN heads  
- Pareto-archive replay for balanced optimization  
- Statistical evaluation with effect size and significance testing  

## Installation
```bash
git clone https://github.com/<your-username>/MARS-HPC.git
cd MARS-HPC
pip install -r requirements.txt

## Datasets
This project uses publicly available HPC workload traces from ALCF.  
Download the datasets here: [ALCF Workload Data](https://reports.alcf.anl.gov/data/index.html).

## Usage
python train.py --config configs/mars.yaml

## Evaluate
python evaluate.py --checkpoint checkpoints/mars.pth

