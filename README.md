# MRT-Rl (Reproduction)

This repository is a reproduction of **MRT-Rl**, primarily based on the following projects:

- [Open-R1](https://github.com/huggingface/open-r1/tree/main)
- [TRL](https://github.com/huggingface/trl/tree/main)
- [unsloth](https://unsloth.ai/blog/r1-reasoning)

## Code Structure
```
src/
├── run.inpnb
└── trl/
    └── trl/
        └── trainer/
            └── grpo_trainer.py
```

## Installation
To set up the environment, please follow the installation instructions provided by the Open-R1 repository.

## Notes
This is an early-stage replication project and may not fully reproduce the original results yet.

Since we need to modify the internal logic of `grpo_trainer.py`, we plan to switch from using the `trl` library as a dependency to importing it locally as part of the codebase.