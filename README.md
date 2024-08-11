# aug-11-agents-hackathon

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

A hackathon project with langchain and fireworks

## Project Organization

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
├── docs               <- A default mkdocs project; see mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for backend
│                         and configuration for tools like black
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
└── backend                <- Source code for use in this project.
    │
    ├── __init__.py    <- Makes backend a Python module
    │
    ├── data           <- Scripts to download or generate data
    │   └── make_dataset.py
    │
    ├── features       <- Scripts to turn raw data into features for modeling
    │   └── build_features.py
    │
    ├── models         <- Scripts to train models and then use trained models to make
    │   │                 predictions
    │   ├── predict_model.py
    │   └── train_model.py
    │
    └── visualization  <- Scripts to create exploratory and results oriented visualizations
        └── visualize.py
```

## Setup Instructions for macOS

Follow these steps to set up the project environment on macOS:

1. **Clone the repository**:

   ```sh
   git clone https://github.com/nehiljain/aug-11-agents-hackathon.git
   cd aug-11-agents-hackathon
   ```

2. **Install Python 3.10**:
   Ensure you have Python 3.10 installed. You can use `pyenv` to manage Python versions:

   ```sh
   brew install pyenv
   pyenv install 3.10.0
   pyenv local 3.10.0
   ```

3. **Set up the virtual environment and install dependencies**:
   Use the `Makefile` to create the virtual environment and install dependencies:

   ```sh
   make install
   ```

4. **Activate the virtual environment**:
   Activate the virtual environment:

   ```sh
   source .venv/bin/activate
   ```

5. **Verify the setup**:
   Ensure everything is set up correctly by running:
   ```sh
   make lint
   ```

You are now ready to start working on the project!

## Available Makefile Commands

- `make install`: Set up the virtual environment and install dependencies.
- `make lint`: Lint the code using `flake8` and `black`.
- `make format`: Format the code using `black`.
- `make data`: Generate the dataset.
- `make clean`: Delete all compiled Python files.

For more details, refer to the `Makefile`.

Composio Apps: [https://app.composio.dev/apps?category=all](https://app.composio.dev/apps?category=all)
