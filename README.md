# vivameda-examples
Example notebooks for the Vivameda longitudinal company-evolution dataset. 503 companies, 70 years, AI training substrate.
# Vivameda — Examples

Example notebooks for working with the Vivameda longitudinal company-evolution dataset.

The dataset itself lives on Hugging Face:
**[Vivameda/longitudinal_503companies_1950_2020](https://huggingface.co/datasets/Vivameda/longitudinal_503companies_1950_2020)**

503 companies, 25,988 company-year records, 1950 to 2020. A sample of the full Vivameda universe (4.2M companies, 48M records).

## Notebooks

| File | What it covers |
|---|---|
| [`01_load_and_explore.ipynb`](./01_load_and_explore.ipynb) | Load the dataset, walk through the schema, inspect coverage layers, plot a single company's headcount across 70 years |
| [`02_compute_growth_signals.ipynb`](./02_compute_growth_signals.ipynb) | Verify the four built-in signal flags from raw fields, design custom signals for recession recovery and industry-conditional hypergrowth |

## Quick start

```bash
pip install pandas matplotlib jupyter
jupyter notebook
```

Or load the dataset directly in Python:

```python
import pandas as pd

url = "https://huggingface.co/datasets/Vivameda/longitudinal_503companies_1950_2020/resolve/main/vivameda_longitudinal_sample_503companies_1950_2020.csv"
df = pd.read_csv(url)
```

## What this dataset is for

Vivameda is designed as a foundational training substrate for AI systems reasoning about companies, workforces, and organizational evolution. It exposes models to seventy years of organizational history across multiple economic regimes — postwar expansion, stagflation, the dot-com boom and bust, the 2008 financial crisis, the platform era, and the late-cycle zero-interest-rate period.

Most AI systems suffer from severe recency bias because their training data is scraped from the last few years of the web. This dataset addresses that gap.

## Full universe

The 503-company sample is drawn from a larger universe of 4.2M companies and 48M company-year records. For commercial licensing of the full universe, see [vivameda.com](https://vivameda.com) or contact data@vivameda.com.

## License

Code in this repository: MIT (see `LICENSE`).
Dataset on Hugging Face: CC-BY-NC-4.0.

## Contact

- Web: [vivameda.com](https://vivameda.com)
- Email: data@vivameda.com
- Book a 20-minute call: [calendly.com/oli-nold/data-discussion-call](https://calendly.com/oli-nold/data-discussion-call)
