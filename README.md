# Learning EDA Dataset

This repository contains datasets for practicing exploratory data analysis in the EDA workshop.

## Dataset List

| Dataset                              | Description                          | Direct Link                          |
| ---------------------------- | ------------------------------------ | ------------------------------------ |
| `pakistan_ecommerce_raw.csv` | Data mentah yang digunakan sebagai dataset awal | https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_raw.csv |
| `pakistan_ecommerce_03.csv`  | Dataset hasil output dari Session 3: Data Cleaning  | https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_03.csv  |
| `pakistan_ecommerce_05.csv`  | Dataset hasil output dari Session 5: Handling Missing Values | https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_05.csv  |

## Dataset Usage Flow

Dataset digunakan secara bertahap sesuai kebutuhan tiap sesi workshop.

| Session | Input Dataset | Keterangan |
| ------- | ------------- | ---------- |
| 2 | `pakistan_ecommerce_raw.csv` | Menggunakan raw dataset untuk eksplorasi awal |
| 3 | `pakistan_ecommerce_raw.csv` | Menggunakan raw dataset sebagai input untuk proses data cleaning |
| 4 | `pakistan_ecommerce_03.csv` | Menggunakan output dataset dari Session 3 sebagai input untuk analisis descriptive statistics |
| 5 | `pakistan_ecommerce_03.csv` | Menggunakan output dataset dari Session 3 sebagai input untuk proses handling missing values |
| 6 | `pakistan_ecommerce_05.csv` | Menggunakan output dataset dari Session 5 sebagai input untuk analisis outliers |

Secara umum, alur dataset adalah sebagai berikut:

```text
pakistan_ecommerce_raw.csv
        │
        ├── Session 2: Data Wrangling & Loading
        └── Session 3: Data Cleaning
                    │
                    ▼
        pakistan_ecommerce_03.csv
                    │
                    ├── Session 4: Descriptive Statistics
                    └── Session 5: Missing Values
                                │
                                ▼
                    pakistan_ecommerce_05.csv
                                │
                                └── Session 6: Outliers
```

## How to Load the Datasets

### Raw Dataset

Raw dataset digunakan sebagai input untuk Session 2 dan Session 3.

```python
import pandas as pd

df = pd.read_csv('https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_raw.csv')
df.head()
```

### Session 3 Output

Dataset ini merupakan output dari Session 3 dan digunakan sebagai input untuk Session 4 dan Session 5.

```python
import pandas as pd

df = pd.read_csv('https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_03.csv')
df.head()
```

### Session 5 Output

Dataset ini merupakan output dari Session 5 dan digunakan sebagai input untuk Session 6.

```python
import pandas as pd

df = pd.read_csv('https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_05.csv')
df.head()
```

## Notes

- Gunakan dataset yang sesuai dengan sesi workshop.
- Dataset hanya boleh diakses melalui link yang sudah tertera pada tabel **Dataset List** di atas.
- Jangan menggunakan dataset pribadi atau file lain di luar link yang sudah disediakan agar hasil analisis antar peserta tetap konsisten.
- Untuk setiap sesi, gunakan input dataset sesuai tabel **Dataset Usage Flow**.
- Dataset output dari sesi sebelumnya digunakan agar peserta dapat melanjutkan materi tanpa harus mengulang seluruh proses dari awal.
