# Data-Science-Learning

## Objective

This repository is a personal data science learning workspace. It summarizes
required skills for data scientists through Obsidian-compatible Markdown notes
and Jupyter notebooks that combine concepts with hands-on practice.

The material currently covers Python fundamentals, dataframe libraries,
statistics, machine learning, deep learning, and time series analysis. New
notebooks should follow the project notebook template:
[utils/Jupyter notebook template.ipynb](utils/Jupyter%20notebook%20template.ipynb).

## Repository Structure

| Path | Description |
| --- | --- |
| [index.md](index.md) | Root index for all study areas. |
| [python/](python/) | Python study materials, including fundamentals, intermediate topics, advanced topics, references, and notebooks. |
| [dataframe/](dataframe/) | Dataframe study materials for NumPy, Pandas, Polars, and PySpark. |
| [statistics/](statistics/) | Statistics study materials. |
| [machin_learning/](machin_learning/) | Machine learning study materials. |
| [deep_learning/](deep_learning/) | Deep learning study materials. |
| [time_series/](time_series/) | Time series study materials. |
| [utils/](utils/) | Shared templates and supporting files. |
| [.github/workflows/](.github/workflows/) | GitHub Actions workflows for repository checks. |
| [pyproject.toml](pyproject.toml) | Python project metadata and dependencies. |
| [uv.lock](uv.lock) | Locked dependency versions managed by `uv`. |

Main topic indexes:

| Topic | Index |
| --- | --- |
| Python | [python/python.md](python/python.md) |
| Dataframe | [dataframe/dataframe.md](dataframe/dataframe.md) |
| Statistics | [statistics/statistics.md](statistics/statistics.md) |
| Machine Learning | [machin_learning/machin_learning.md](machin_learning/machin_learning.md) |
| Deep Learning | [deep_learning/deep_learning.md](deep_learning/deep_learning.md) |
| Time Series | [time_series/time_series.md](time_series/time_series.md) |

## Prerequisites and Set-Up

Prerequisites:

- Python 3.12 or later
- `uv` for Python environment and dependency management
- A Jupyter-capable editor or runtime, such as VS Code, JupyterLab, or Jupyter
  Notebook

Set up the repository:

```bash
git clone <repository-url>
cd Data-Science-Learning
uv sync
```

Register the project virtual environment as a Jupyter kernel:

```bash
uv run ipython kernel install --user --env VIRTUAL_ENV "$(pwd)/.venv" --name data-science-learning --display-name "Data Science Learning"
```

After registration, select the `Data Science Learning` kernel when opening
notebooks.

If `uv` is not installed, install it first by following the official `uv`
installation guide.

## How to Run Notebooks

1. Open this repository in VS Code, JupyterLab, or Jupyter Notebook.
2. Start from [index.md](index.md) or a topic index to choose a notebook.
3. Open the `.ipynb` file.
4. Select the `Data Science Learning` kernel.
5. Run notebook cells from top to bottom.

Example notebooks:

- [python/Introduction - Why Python.ipynb](python/Introduction%20-%20Why%20Python.ipynb)
- [python/fundamental/Python fundamental - Function.ipynb](python/fundamental/Python%20fundamental%20-%20Function.ipynb)
- [dataframe/NumPy/fundamental/NumPy fundamental - Overview.ipynb](dataframe/NumPy/fundamental/NumPy%20fundamental%20-%20Overview.ipynb)

For additional kernel setup notes, see
[python/How to enable jupyter notebook kernel.md](python/How%20to%20enable%20jupyter%20notebook%20kernel.md).

* Materials are created with the support of Codex.
