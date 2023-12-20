# python-project-template
Simple python project template

# Deploy project with Flit
[Flit](https://flit.pypa.io/en/stable/index.html) uses `pyproject.toml` for configuration and `.pypirc` for deployment location.
- Install flit: `pip install flit`
- Install project locally for development: `flit install`
- Publish project to PyPI: `flit publish`
- Publish project to testPyPI: `flit publish --repository testpypi`
