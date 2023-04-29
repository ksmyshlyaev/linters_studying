## Installation guide for black and isort

1. Install latest versions of `black`, `isort` and `pre-commit` packages into virtual environment
2. Create `.pre-commit-config.yaml` file and specify `black` and `isort`
   repos as described. Specified versions should match the package versions
   that were installed to virtual environment
3. Create `pyproject.toml` file, (optionally) specify `[tool.black]` clause and specify `[tool.isort]` clause with
   `profile = "black"`
4. Run `pre-commit install` command

Now both `black` and `isort` tools will work simultaneously before each commit and will not conflict with each other.