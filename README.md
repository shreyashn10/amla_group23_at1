# amla_group23_at1

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

Repository for assignment 1 of Adv. Machine Learning.

## Project Setup and Usage Guide
Welcome to the amla_group23_at1 project! This guide will walk you through setting up your environment to run the project.

### Prerequisites
Before you begin, please ensure the following software is installed on your system:

**Python**: A recent version of Python is required.

**pyenv**: This tool manages Python versions. For installation instructions, see https://realpython.com/lessons/installing-pyenv/.

**Poetry**: The dependency management tool for this project. For installation instructions, see https://python-poetry.org/docs/#installation.

**Wget** (for Windows users): A utility for non-interactive file downloading. For installation instructions, see https://eternallybored.org/misc/wget/.

### Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is the subject of class,
│                         the group ID, StudentID, AssignmentID, and experiment number (for ordering), e.g.
│                         `36120-25SP-group1-149874-AT1-experiment-1.ipynb`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         amla_group23_at1 and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── amla_group23_at1   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes amla_group23_at1 a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------

### Getting Started
Follow these steps to initialize the project environment and start working:

1. **Download and Extract**: Download the repository and extract the contents into your desired directory.

2. **Open Terminal**: Navigate to the root of the project folder using your terminal or command prompt.

3. **Install Python Version**: Use ```pyenv``` to install the required Python version.
```

pyenv install 3.11.4

```
4. **Set Local Python**: Set the local Python version for this project to ```3.11.4```
```

pyenvv local 3.11.4

```
5. **Install Dependencies**: Use Poetry to install all the necessary packages listed in ```pyproject.toml```.
```

poetry install

```
6. **Activate Virtual Environment**: Activate the project's virtual environment. All subsequent commands should be run from within this terminal.
```

poetry env activate

```
7. **Open Jupyter Lab**: Launch Jupyter Lab to access the notebooks for running experiments.
```

poetry run jupyter lab

```
8. **Add Your Data**: Upload your raw data (.CSV file) into the ```data/raw``` folder of the project.

9. **Run Experiments**: Open and run the notebooks located in the ```notebooks``` folder to run experiments and analysis.