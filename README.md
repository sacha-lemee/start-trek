# START TREK

![START TREK](doc/lunar_lander.gif)

### Development

By *Ariel Amriou*(ariel.amriou@epitech.eu), *Pierrick Simon*(pierrick.simon@epitech.eu) & *Sacha Lemée*(sacha.lemee@epitech.eu).

## Objective

Train a Lunar Lander agent using Reinforcement Learning to autonomously land safely on the Moon (Gymnasium LunarLander-v3 environment).

- "You will program an algorithm that enables the module to correct its own trajectory. It will be a reinforcement-learning agent that learns by trial and error from sparse rewards" *(From the START TREK EPITECH subject)*

**Success criteria:** score > 200 over 100 consecutive episodes.

## Getting Started

### Prerequisites

This project requires:
- Python 3.12 and pip
- Gymnasium and PyTorch (installed from `requirements.txt`)
- Box2D, the physics engine of the environment (built by pip, see step 3)

### Installation for Linux

1. **Clone the repository:**

```sh
git clone git@github.com:sacha-lemee/start-trek.git
```

2. **Navigate to the project directory:**

```sh
cd start-trek
```

3. **Install the dependencies:**

```sh
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

*Box2D is built from source by pip: if the install fails, install `swig` and a C/C++ compiler first (`sudo apt install swig build-essential`).*

4. **Run an experiment:**

Each run is described by a YAML file (algorithm, training or evaluation mode, hyperparameters). A commented example is provided in [`doc/example.yaml`](doc/example.yaml):

```sh
python3 startTrek.py doc/example.yaml
```

Results (CSV, videos) are written to `data_<algo>/`. To plot a run:

```sh
./review.py data_dqn
```

5. **Reproduce the full experiment:**

```sh
./reproduce.sh
```

It trains Q-Learning (`configs/qlearn.yaml`) and DQN (`configs/dqn.yaml`), evaluates a random baseline (`configs/random.yaml`) and generates the plots with `review.py`. The DQN hyperparameters are the ones described in the report.

## Documentation

See the [START TREK report](doc/G-AIA-401_start_trek_Report.pdf) (in French): algorithms, results and ablation study.

## Epitech warning

This project was built for the Epitech curriculum. **Epitech students: do not copy this code for your own project.** Copying is forbidden at Epitech and is treated as cheating. Read it to learn if you want, but write your own.

## Contributing

Contributions are welcome: read [CONTRIBUTING.md](CONTRIBUTING.md) and the [code of conduct](CODE_OF_CONDUCT.md).

## License

This project is licensed under the **MIT License**, see [LICENSE](LICENSE).

![START TREK License : MIT](https://img.shields.io/badge/License-MIT-blue.svg)
