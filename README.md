# PPO from Scratch

A complete implementation of the Proximal Policy Optimization (PPO) algorithm from scratch, compatible with OpenAI Gym/Gymnasium API.

## Features

- **Gymnasium Compatible**: Compatible with any Gymnasium environment (discrete or continuous)
- **Training Utilities**: Includes training scripts with progress tracking and visualization
- **Model Persistence**: Save and load trained models with automatic compatibility checking

## Installation

1. Clone the repository:
```bash
git clone https://github.com/minsoo0926/PPO_scratch.git
cd PPO_scratch
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Quick Start

### Basic Usage

### Using the Training Script
- Modify config.py as your training environment
```bash
make train
make test
```

## File Structure

```
PPO_scratch/
├── ppo/                     # Main PPO implementation
├── models/                  # Saved models
├── train.py                 # Training script  
├── example.py               # Usage example
└── config.py                # Configuration
```

## Supported Environments

**Automatic compatibility** with Gymnasium environments:
- **Discrete**: `gym.spaces.Discrete` → `DiscretePPOAgent`  
- **Continuous**: `gym.spaces.Box` → `ContinuousPPOAgent`

**Tested**: CartPole-v1, LunarLander-v2, Pendulum-v1, BipedalWalker-v3, Ant-v5, Humanoid-v5
