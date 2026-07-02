# Topsis-Gautam-102203498

A Python implementation of the **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution) multi-criteria decision-making method, published to PyPI as [`Topsis-Gautam-102203498`](https://pypi.org/project/Topsis-Gautam-102203498/).

TOPSIS ranks alternatives by their distance from an ideal-best and ideal-worst solution: the best alternative has the shortest distance from the ideal-best and the longest distance from the ideal-worst.

## Install

```bash
pip install Topsis-Gautam-102203498
```

## Usage

```bash
python 102203498.py.py <inputFile.csv> <weights> <impacts> <resultFile.csv>
```

- `inputFile.csv` — a CSV with an identifier column followed by numeric criteria columns.
- `weights` — comma-separated weights for each criterion, e.g. `1,1,1,2`.
- `impacts` — comma-separated `+`/`-` for each criterion (`+` = higher is better, `-` = lower is better), e.g. `+,+,-,+`.
- `resultFile.csv` — output path; the input data with added `Topsis Score` and `Rank` columns.

## Example

```bash
python 102203498.py.py 102203498-data.csv "1,1,1,1" "+,+,-,+" 102203498-result.csv
```

## Project structure

| File | Purpose |
|---|---|
| `102203498.py.py` | Core TOPSIS implementation (CLI entry point) |
| `__init__.py` | Package entry point (same core logic, exposed for import) |
| `102203498_Gautam_topsis_text.py` | Extended example applying TOPSIS to rank sentence-embedding models |
| `102203498-data.csv` | Sample input data |
| `102203498-result.csv` | Sample output with scores and ranks |
