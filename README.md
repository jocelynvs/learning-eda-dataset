# Learning EDA Dataset

This repository contains datasets for practicing exploratory data analysis in the EDA workshop.

## Dataset List

| Dataset                              | Description                                                    | File                         | Direct Link                                                                                       |
| ------------------------------------ | -------------------------------------------------------------- | ---------------------------- | ------------------------------------------------------------------------------------------------- |
| Pakistan Ecommerce Raw Dataset       | Raw data that will be processed during the EDA workshop        | `pakistan_ecommerce_raw.csv` | [Download](https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_raw.csv) |
| Pakistan Ecommerce Session 3 Dataset | Output dataset from material session 3: data cleaning          | `pakistan_ecommerce_03.csv`  | [Download](https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_03.csv)  |
| Pakistan Ecommerce Session 4 Dataset | Output dataset from material session 4: descriptive statistics | `pakistan_ecommerce_04.csv`  | [Download](https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_04.csv)  |
| Pakistan Ecommerce Session 5 Dataset | Output dataset from material session 5: missing values         | `pakistan_ecommerce_05.csv`  | [Download](https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_05.csv)  |

## How to Load the Datasets

### Raw Dataset

```python
import pandas as pd

url = "https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_raw.csv"

df_raw = pd.read_csv(url)
df_raw.head()
```

### Session 3 Output: Data Cleaning

```python
import pandas as pd

url = "https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_03.csv"

df_session_3 = pd.read_csv(url)
df_session_3.head()
```

### Session 4 Output: Descriptive Statistics

```python
import pandas as pd

url = "https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_04.csv"

df_session_4 = pd.read_csv(url)
df_session_4.head()
```

### Session 5 Output: Missing Values

```python
import pandas as pd

url = "https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_05.csv"

df_session_5 = pd.read_csv(url)
df_session_5.head()
```
