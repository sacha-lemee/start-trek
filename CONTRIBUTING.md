# Contributing to START TREK

START TREK was built by a fixed team during the Epitech curriculum. Issues and pull requests are welcome.

## Project layout

`startTrek.py` reads a YAML config and runs `src/main.py`. The agents are in `src/` (`qlearn.py`, `dqn.py`, `random.py`), the training and evaluation loops in `train.py` and `eval.py`. Configs are in `configs/`. See the [README](README.md) to build and run it.

## Workflow

1. Open an issue describing the bug or the change.
2. Create a branch from `main`: named after the topic, like the existing `Discretisation` or `Reproduce` branches.
3. Commit with the convention of the history: `type: summary` or `type(Scope): summary`, e.g. `feat: add of random baseline`.
4. Open a pull request into `main` with a short list of the changes and `Closes #<issue>`.

## Code style

- Python 3.12.
- Hyperparameters come from the YAML configs, never from the code.
- Do not commit the `data_*` folders: they hold generated CSV files, models and videos.

## Code of conduct

By contributing you agree to follow the [code of conduct](CODE_OF_CONDUCT.md).
