# Prima

This repository is fine-tuned to conse multi-agent tasks, we also recommend an optimized implementation of QMIX: https://github.com/marlbenchmark/off-policy.


## Finetuned-QMIX

There are so many code-level tricks in the  Multi-agent Reinforcement Learning (MARL), such as:
- Value function clipping (clip max Q values for QMIX)
- Value Normalization
- Reward scaling

**Related Works**

- Implementation Matters in Deep RL: A Case Study on PPO and TRPO
- What Matters In On-Policy Reinforcement Learning? A Large-Scale Empirical Study
- The Surprising Effectiveness of MAPPO in Cooperative, Multi-Agent Games

# Usage
Prima is framework for deep multi-agent reinforcement learning and includes implementations of the following algorithms:

Value-based Methods:

- [**QMIX**: QMIX: Monotonic Value Function Factorisation for Deep Multi-Agent Reinforcement Learning]
- [**VDN**: Value-Decomposition Networks For Cooperative Multi-Agent Learning]
- [**IQL**: Independent Q-Learning]


## Installation instructions

Install Python packages

```shell
# require Anaconda 3 or Miniconda 3
conda create -n pymarl python=3.8 -y
conda activate pymarl

bash install_dependecies.sh
```

Set up 

```shell
bash install_sc2.sh
```

## Command Line Tool

**Run an experiment**

```shell

python3 src/main.py --config=qmix --env-config=sc2 with env_args.map_name=corridor
```

```shell
# For Communication tasks
python3 src/main.py --config=qmix_att --env-config=sc2 with env_args.map_name=1o_10b_vs_1r
```
