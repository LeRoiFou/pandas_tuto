# Librairie Pandas

Possibilité d'effectuer des traitements similaires à la librairie pandas, mais avec des instructions plus simples avec la librairie [sidetable](https://github.com/chris1610/sidetable). <br>
[Lien expliquant l'intérêt de la librairie sidetable](https://www.linkedin.com/feed/update/urn:li:activity:7204414221852356610/)

---

Il est préférable de travailler sur un fichier au format Parquet que sur un fichier au format CSV pour une meilleure efficacité de stockage : Parquet peut réduire la taille du fichier jusqu'à 10 fois par rapport au CSV.

```
import pandas as pd

# Lecture du fichier CSV
df = pd.read_csv("votre_fichier.csv")

# Conversion en Parquet
df.to_parquet("votre_fichier.parquet", engine="pyarrow", index=False)

# Lecture du fichier Parquet
df_parquet = pd.read_parquet("votre_fichier.parquet")
```

Date : 11/02/2025
