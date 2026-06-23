# Learning EDA Dataset

This repository contains datasets for practicing exploratory data analysis in the EDA workshop.

## Dataset List

| Dataset                              | Description                                           | Direct Link                                                                                       |
| ------------------------------------ | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `pakistan_ecommerce_raw.csv`       | Data mentah yang digunakan sebagai dataset awal | https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_raw.csv |
| `pakistan_ecommerce_03.csv` | Dataset hasil output dari Session 3: Data Cleaning  | https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_03.csv  |
| `pakistan_ecommerce_05.csv`  | Dataset hasil output dari Session 5: Handling Missing Values | https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_05.csv  |

## Dataset Usage Flow

Dataset digunakan secara bertahap sesuai kebutuhan tiap sesi workshop.

| Session | Input Dataset | Keterangan |
| ------- | ------------- | ---------- |
| Session 2 | `pakistan_ecommerce_raw.csv` | Menggunakan raw dataset untuk eksplorasi awal |
| Session 3 | `pakistan_ecommerce_raw.csv` | Menggunakan raw dataset sebagai input untuk proses data cleaning |
| Session 4 | `pakistan_ecommerce_03.csv` | Menggunakan output dari Session 3 sebagai input analisis berikutnya |
| Session 5 | `pakistan_ecommerce_03.csv` | Menggunakan output dari Session 3 sebagai input untuk materi handling missing values |
| Session 6 | `pakistan_ecommerce_05.csv` | Menggunakan output dari Session 5 sebagai input untuk analisis lanjutan |

Secara umum, alur dataset adalah sebagai berikut:

```text
pakistan_ecommerce_raw.csv
        │
        ├── Session 2
        └── Session 3: Data Cleaning
                    │
                    ▼
        pakistan_ecommerce_03.csv
                    │
                    ├── Session 4
                    └── Session 5: Handling Missing Values
                                │
                                ▼
                    pakistan_ecommerce_05.csv
                                │
                                └── Session 6
```

## How to Load the Datasets

### Raw Dataset

Raw dataset digunakan sebagai input untuk Session 2 dan Session 3.

```python
import pandas as pd

url = "https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_raw.csv"

df_raw = pd.read_csv(url)
df_raw.head()
```

### Session 3 Output: Data Cleaning

Dataset ini merupakan output dari Session 3 dan digunakan sebagai input untuk Session 4 dan Session 5.

```python
import pandas as pd

url = "https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_03.csv"

df_session_3 = pd.read_csv(url)
df_session_3.head()
```

### Session 5 Output: Handling Missing Values

Dataset ini merupakan output dari Session 5 dan digunakan sebagai input untuk Session 6.

```python
import pandas as pd

url = "https://github.com/jocelynvs/learning-eda-dataset/raw/main/pakistan_ecommerce_05.csv"

df_session_5 = pd.read_csv(url)
df_session_5.head()
```

## Notes

- Gunakan dataset yang sesuai dengan sesi workshop.
- Dataset hanya boleh diakses melalui link yang sudah tertera pada tabel **Dataset List** di atas.
- Jangan menggunakan dataset pribadi atau file lain di luar link yang sudah disediakan agar hasil analisis antar peserta tetap konsisten.
- Untuk setiap sesi, gunakan input dataset sesuai tabel **Dataset Usage Flow**.
- Dataset output dari sesi sebelumnya digunakan agar peserta dapat melanjutkan materi tanpa harus mengulang seluruh proses dari awal.
