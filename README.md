# Parkinsons Telemonitoring

Explores how well voice measurements predict motor and total UPDRS scores using k-nearest neighbors regression. The [Jupyter notebook](parkinsons_telemonitoring_analysis.ipynb) contains the analysis, model explanations, results, and limitations. The [HTML report](parkinsons_telemonitoring_analysis.html) can be opened in a browser without running Python.

## Requirements

- uv 0.12+

## Running the notebook

From the project folder:

```bash
uv sync --locked
uv run jupyter lab
```

Open `parkinsons_telemonitoring_analysis.ipynb`, restart the kernel, and run all cells in order. Save the notebook to retain its results and plots.

To update the HTML report after saving:

```bash
uv run jupyter nbconvert --to html parkinsons_telemonitoring_analysis.ipynb
```

## Dataset

The [Parkinsons Telemonitoring dataset](https://archive.ics.uci.edu/dataset/189/parkinsons+telemonitoring) comes from the UCI Machine Learning Repository and contains 5,875 voice recordings from 42 participants.

- [`data/parkinsons_updrs.data`](data/parkinsons_updrs.data): the dataset in CSV format.
- [`data/parkinsons_updrs.names`](data/parkinsons_updrs.names): the accompanying dataset documentation.

Tsanas, A., & Little, M. (2009). *Parkinsons Telemonitoring* [Dataset]. UCI Machine Learning Repository. [doi:10.24432/C5ZS3N](https://doi.org/10.24432/C5ZS3N).
