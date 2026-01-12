This repository contains code and sample datasets for **airport gate and stand assignment**, including both **initial allocation** (with Graph Neural Networks, GNNs) and **dynamic reassignment** under delays (with Deep Reinforcement Learning, PPO/DQN).

## Week 1
- `Stand_assignment.ipynb`

  Pre-allocation and Dynamic Gate Reallocation intial trial.
  
Method: GCN

## Week 2
- `schiphol_flights_2025-08-01.csv`

  Initially use Python to obtain Schiphol Airport data.
  
  Initial GNN trial on the dataset.
  
Method: GNN
  
## Week 3
- `schiphol_flights_20250701_20250731.csv`, `schiphol_flights_cleaned_20250710.csv`, `final_filled_result.csv`
  
  Example flight data for **Amsterdam Schiphol (AMS)**. 
- `schiphol_flights_clean_and_stand_assignment.ipynb`
  
  Clean data. Simulate stand info and filght pair based on exist info (but many problems).
- `GNN_based_gate_assignment.ipynb`
  
  Use GNN to pre allocate stand and gates for schiphol airport.
  
Method: GNN

## Week 4
- `SFO_Gate_and_Stand_Assignment_Information.csv`
  
  Find new data for **San Francisco (SFO)**.
- `simulated_flight_gate_assignment.csv`
  
  Simulation outputs or post-processed assignment results.
- `Simulated_DRL_Gate_Assignment.ipynb`
  
  End-to-end DRL simulation environment: observation/action spaces, reward design, training curves, evaluation.
  
Method: PPO

Initial trial on PPO for real time allocation.

## Week 5
- `DRL_PPO_Gate_Assignment.ipynb`
- `DRL_DQN_gate_assignment.ipynb`
- `GNN+PPO.ipynb`
- `GNN+DQN.ipynb`
- `PPO_reassignment result.csv`
  
Method: PPO, DQN, GNN

Work done: Add total_timesteps

The following methods were compared based on simulated data: PPO, DQN, GNN(pre_allocation) + PPO(real time), GNN(pre_allocation) + GQN(real time)

## Week 6
- `SAT_airport_PPO_gate_assignment.ipynb`
  
Method: PPO

Work done: Add more constraints 

Combined with SAT airport actual layout simulation data, and applied DRL PPO to perform real-time redistribution in situations of flight delays.

Environment Setup

- Python 3
- Recommended dependencies:
  - `pandas`, `numpy`, `matplotlib`
  - `torch`, `torch-geometric` (for GNNs)
  - `stable-baselines3` (for PPO/DQN)
  - `jupyterlab` or `notebook`

## 12/1/2026

Have done some experiments on SFO (large) and SAT (small) airport. Recorded on file `SAT experiment (small airport).docx` and `SFO experiment (large airport).docx`. Upload Python file `V7_SFO_gate_assignment.ipynb` and `V9_SAT_airport_3_way_gate_assignment.ipynb`.
