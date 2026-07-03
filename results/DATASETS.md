# Datasets used in this research

All three datasets are publicly available on [OpenML](https://www.openml.org) and are fetched automatically by the notebook via `sklearn.datasets.fetch_openml`. No manual download is required.

## Dataset 1: Blood Transfusion Service Center

- **OpenML ID:** 1464
- **URL:** https://www.openml.org/d/1464
- **Samples:** 748
- **Features:** 4 (recency, frequency, monetary, time)
- **Classes:** 2 (binary)
- **Minority %:** 23.80
- **Domain:** Medical (blood donation)

## Dataset 2: Wisconsin Diagnostic Breast Cancer (WDBC)

- **OpenML ID:** 1510
- **URL:** https://www.openml.org/d/1510
- **Samples:** 569
- **Features:** 30 (numerical, derived from digitized FNA images)
- **Classes:** 2 (binary — malignant/benign)
- **Minority %:** 37.26
- **Domain:** Medical (oncology)

## Dataset 3: EEG Eye State

- **OpenML ID:** 1471
- **URL:** https://www.openml.org/d/1471
- **Samples:** 14,980
- **Features:** 14 (EEG channels)
- **Classes:** 2 (binary — eye open/closed)
- **Minority %:** 44.88
- **Domain:** Medical (neuroscience)

## Loading Code

```python
from sklearn.datasets import fetch_openml

# Dataset 1: Blood Transfusion
ds1 = fetch_openml(data_id=1464, as_frame=True, parser='auto')

# Dataset 2: WDBC Breast Cancer
ds2 = fetch_openml(data_id=1510, as_frame=True, parser='auto')

# Dataset 3: EEG Eye State
ds3 = fetch_openml(data_id=1471, as_frame=True, parser='auto')
```

## License

All three datasets are publicly available and licensed for research use. See OpenML's dataset pages for specific license information.
