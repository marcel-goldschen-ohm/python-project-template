# python-project-template
Simple python project template

# Project hierarchy
```
/
├── src/
│   └── mypackage/
│       ├── __init__.py
│       └── mymodule.py
├── tests/
│   └── test_something.py
├── README.md
├── LICENSE
├── pyproject.toml
└── .pypirc
```

# Deploy project with Flit
[Flit](https://flit.pypa.io/en/stable/index.html) uses `pyproject.toml` for configuration and `.pypirc` for deployment to [PyPI](https://pypi.org).

Run flit commands in the project directory.
- Install flit: `pip install flit`
- Install project locally for development: `flit install`
- Publish project to PyPI: `flit publish`
- Publish project to testPyPI: `flit publish --repository testpypi`
