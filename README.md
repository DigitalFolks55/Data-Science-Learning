# Data-Science-Learning

## 1. Overall

This repository is a personal learning notebook for data science topics. It
collects Markdown notes and Jupyter notebooks covering Python fundamentals,
dataframes, statistics, machine learning, deep learning, and time series.

The contents are organized as study indexes so each topic can grow over time.
Some content was generated or refined in collaboration with ChatGPT.

## 2. Contents

| Topic | Path | Description |
| --- | --- | --- |
| Main index | [index.md](index.md) | Root index for all study areas. |
| Python | [python/python.md](python/python.md) | Python fundamentals, intermediate and advanced notes, notebooks, and references. |
| Dataframe | [dataframe/dataframe.md](dataframe/dataframe.md) | Index for dataframe study notes. |
| Statistics | [statistics/statistics.md](statistics/statistics.md) | Index for statistics study notes. |
| Machine Learning | [machin_learning/machin_learning.md](machin_learning/machin_learning.md) | Index for machine learning study notes. |
| Deep Learning | [deep_learning/deep_learning.md](deep_learning/deep_learning.md) | Index for deep learning study notes. |
| Time Series | [time_series/time_series.md](time_series/time_series.md) | Index for time series study notes. |

Notebooks are currently stored under the `python/` directory, including Python
introduction and fundamental syntax notebooks.

## 3. Environment Set-Up

This project uses Python 3.12 and `uv` for environment and dependency
management.

1. Clone the repository and move into it.

   ```bash
   git clone <repository-url>
   cd Data-Science-Learning
   ```

2. Create or sync the virtual environment.

   ```bash
   uv sync
   ```

3. Register the project environment as a Jupyter kernel.

   ```bash
   uv run ipython kernel install --user --env VIRTUAL_ENV "$(pwd)/.venv" --name data-science-learning --display-name "Data Science Learning"
   ```

4. In VS Code or Jupyter, select the `Data Science Learning` kernel when opening
   notebooks.

If `uv` is not installed, install it first by following the official `uv`
installation guide.

## 4. How to Use

Start from [index.md](index.md), then open the topic index for the area you want
to study. For Python, use [python/python.md](python/python.md) to navigate to
fundamental, intermediate, advanced, reference, and notebook materials.

To run the sample Python entry point:

```bash
uv run python main.py
```

To work with notebooks, open an `.ipynb` file and select the registered
`Data Science Learning` kernel.

GitHub Actions runs `.github/workflows/ci.yaml` on push and pull request. The CI
job clears Jupyter notebook outputs and fails if notebook changes other than
outputs are detected.
