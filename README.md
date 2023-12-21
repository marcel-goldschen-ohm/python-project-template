# python-project-template

1. Use a conda environment: `conda create -n myenv python; conda activate myenv`
2. Install poetry: `pip install pipx; pipx install poetry`
3. Create package: `poetry new mypackage` (or `poetry init` in existing package)
4. Add dependencies: `poetry add numpy`
5. Add dependencies for testing: `poetry add pytest --group test`
6. Install mypackage locally for dev: `poetry install`

# OLD
Template for a simple python project.

# Project hierarchy
```
/
├── src/
│   └── mypackage/
│       ├── __init__.py
│       └── mymodule.py
├── tests/
│   └── test_something.py
├── LICENSE
├── README.md
├── pyproject.toml
├── .gitignore
└── .pypirc
```

# Deploy project with Flit
[Flit](https://flit.pypa.io/en/stable/index.html) uses `pyproject.toml` for configuration and `.pypirc` for deployment to [PyPI](https://pypi.org).

Run flit commands in the project directory.
- Install flit: `pip install flit`
- Install project locally for development: `flit install`
- Publish project to PyPI: `flit publish`
- Publish project to testPyPI: `flit publish --repository testpypi`

# Project files
- `src/`: Contains all package directories.
- `tests/`: Contains all test modules.
- `pyproject.toml`: Defines project configurations and dependencies.
- `.pypirc`: Used by flit for deployment to PyPI. *In my opinion this should be done away with and flit should provide its own option to publish to testpypi or some URL.*
