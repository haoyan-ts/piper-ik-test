# Piper IK Test

A Jupyter notebook project for robot kinematics using Pinocchio.

## Project Structure

```
piper-ik-test/
├── notebooks/              # Jupyter notebooks
│   ├── 01_example.ipynb   # Basic data analysis example
│   └── 02_pinocchio_example.ipynb  # Robot kinematics example
├── piper_ik_test/         # Main package directory
│   └── __init__.py
├── tests/                 # Test directory
├── data/                  # Data directory
├── pyproject.toml         # Project configuration and dependencies
└── README.md
```

## Setup

1. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install the package in development mode:
```bash
pip install -e ".[dev]"  # Install with development dependencies
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

## Development

This project uses modern Python packaging with `pyproject.toml`. Key features:

- **Dependency Management**: All dependencies are specified in `pyproject.toml`
- **Development Tools**: Includes development dependencies for testing and code quality
  - `pytest` for testing
  - `black` for code formatting
  - `isort` for import sorting
  - `flake8` for linting

### Development Commands

```bash
# Format code
black .
isort .

# Run tests
pytest

# Run linter
flake8
```

## Getting Started

1. Open `notebooks/01_example.ipynb` to see a basic data analysis example
2. Open `notebooks/02_pinocchio_example.ipynb` to see robot kinematics examples using Pinocchio
3. Create new notebooks in the `notebooks/` directory
4. Store your datasets in the `data/` directory

## Pinocchio Library

This project includes the Pinocchio library for robot kinematics and dynamics. The example notebook demonstrates:
- Creating a simple robot model
- Computing forward kinematics
- Visualizing robot configurations

For more information about Pinocchio, visit: https://github.com/stack-of-tasks/pinocchio 