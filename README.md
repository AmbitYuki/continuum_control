# Subequivariant Collaborative Control for Continuum Robots

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/AmbitYuki/continuum-control?style=social)](https://github.com/AmbitYuki/continuum-control/stargazers)

This repository contains the official implementation of "Latent Dynamics Subequivariant and Context-Aware Variational Collaborative Control for Continuum Robots with Multi-Objective Optimization" from our paper.

## Features

- 🤖 Subequivariant collaborative control framework for continuum robots
- 🧠 Context-aware trajectory encoding via STLDE (Spatio-Temporal Latent Dynamics Encoder)
- 🎯 Multi-objective optimization for balanced control strategies
- 📊 Comprehensive evaluation tools and visualization
- 🔄 Real-world deployment support

## Project Structure

```
.
├── env/                    # Environment configurations and wrappers
├── mbpo/                   # Model-based policy optimization
├── real_world/            # Real-world deployment utilities
├── replay_pools/          # Experience replay implementation
├── scripts/               # Training and evaluation scripts
├── softlearning/          # Core learning algorithms
├── track_encoder/         # Trajectory encoding modules
├── utils/                 # Utility functions
├── value_functions/       # Value function implementations
└── run{1,2,3,4}.py       # Main training scripts
```

## Installation

```bash
# Clone the repository
git clone https://github.com/AmbitYuki/continuum-control.git
cd continuum-control

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
# or
.\venv\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt
```

## Quick Start

1. Train the model:
```bash
python run1.py --config configs/default.yaml
```

2. Evaluate performance:
```bash
python run2.py --model_path checkpoints/best_model.pt
```

3. Real-world deployment:
```bash
python run3.py --hardware_config configs/hardware.yaml
```

## Results

Our framework achieves state-of-the-art performance across multiple metrics:

- 84% reduction in positional error
- 84% reduction in velocity deviation
- 65% reduction in energy consumption
- 58% improvement in success rate


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

We thank the MuJoCo team for providing the physics simulation environment and all contributors to this project.



---
⭐️ If you find this repository helpful, please consider giving it a star!
