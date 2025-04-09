# MRT-Rl (Reproduction)

This repository is a reproduction of **MRT-Rl**, primarily based on the following projects:

- [Open-R1](https://github.com/huggingface/open-r1/tree/main)
- [TRL](https://github.com/huggingface/trl/tree/main)
- [unsloth](https://unsloth.ai/blog/r1-reasoning)

## Code Structure
```
src/
├── DeepSeek-R1-Distill-Qwen-7B_GRPO_run.ipynb
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

- `DeepSeek-R1-Distill-Qwen-7B_origin.ipynb` shows the evaluation of original 7B base model without RLtraining.
- `DeepSeek-R1-Distill-Qwen-1.5B_GRPO_my.ipynb` shows the evaluation of 7B base model after RL training.
- `grpo_trainer_new_ref.py` shows the reference modification for MRT version of `grpo_trainer`.
