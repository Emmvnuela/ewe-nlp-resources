# 🌍 ewe-nlp-resources

> Open resources for the **Ewe (Eʋegbe)** language: parallel sentences, learning notebooks and documentation.
> *Bringing world-class data science TO Africa and FROM Africa to the world.*

![License: CC BY 4.0](https://img.shields.io/badge/data-CC%20BY%204.0-lightgrey)
![License: MIT](https://img.shields.io/badge/code-MIT-blue)
![Status](https://img.shields.io/badge/status-work%20in%20progress-orange)

**Langues / Languages:** [Français](#-en-français) · [English](#-in-english)

---

## 🇫🇷 En français

### Pourquoi ce projet ?
L'éwé est parlé par des millions de personnes au Togo, au Ghana et au Bénin, mais il reste très peu représenté dans les données utilisées pour entraîner les modèles d'IA. Ce dépôt vise à **créer et partager des ressources ouvertes** pour l'éwé, et à **documenter mon apprentissage** de la data science en public.

### Contenu
| Dossier / fichier | Description |
|---|---|
| `data/sentences.csv` | Phrases parallèles éwé – français – anglais |
| `data/DATASHEET.md` | Fiche descriptive du jeu de données (origine, validation, limites) |
| `notebooks/` | Notebooks d'analyse et d'apprentissage (à venir) |
| `journal.md` | Journal d'apprentissage, semaine par semaine |
| `CONTRIBUTING.md` | Comment contribuer |

### Format des données
Fichier CSV encodé en **UTF-8**, avec les colonnes :

| Colonne | Description |
|---|---|
| `id` | Identifiant unique |
| `ewe` | Phrase en éwé |
| `french` | Traduction en français |
| `english` | Traduction en anglais |
| `source` | Origine (ex. : écrit par moi, Tatoeba, etc.) |
| `validated` | `yes` si relue par une locutrice/un locuteur natif, sinon `no` |

### Utiliser les données
```python
import pandas as pd

df = pd.read_csv("data/sentences.csv", encoding="utf-8")
print(df.head())
```

### Feuille de route
- [ ] Première version du jeu de données (50 phrases)
- [ ] Datasheet complète
- [ ] Premier notebook : analyse exploratoire (longueur des phrases, vocabulaire)
- [ ] Atteindre 500 phrases validées
- [ ] Contribuer ces données à des projets communautaires (Masakhane, Tatoeba…)

### Licences
- **Données** : [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.fr) — tu peux les réutiliser en citant ce dépôt.
- **Code** : MIT.

### Contribuer
Les contributions sont les bienvenues, surtout celles de **locuteurs natifs** : ajout de phrases, relecture, corrections. Voir [CONTRIBUTING.md](CONTRIBUTING.md).

### Citer ce projet
```
Afi Emmanuela Carlos AGBEKPONOU. (2026). ewe-nlp-resources: open Ewe–French–English parallel sentences.
GitHub. https://github.com/Emmvnuela/ewe-nlp-resources
```

### À propos de moi
Je suis Afi, locutrice native de l'éwé, passionnée par la data science pour les contextes africains. Je débute et j'apprends en public. Retrouve-moi sur [GitHub](https://github.com/Emmvnuela) · [Linkedin](www.linkedin.com/in/emmanuela-agbekponou-afi).

---

## 🇬🇧 In English

### Why this project?
Ewe is spoken by millions of people in Togo, Ghana and Benin, yet it is barely represented in the data used to train AI models. This repository aims to **create and share open resources** for Ewe and to **document my data science learning journey** publicly.

### Contents
See the table above. The main dataset is `data/sentences.csv` (Ewe–French–English parallel sentences, UTF-8), described in `data/DATASHEET.md`.

### Licenses
Data: CC BY 4.0. Code: MIT.

### Contributing
Contributions are welcome, especially from **native Ewe speakers**: adding sentences, reviewing translations, fixing errors. See [CONTRIBUTING.md](CONTRIBUTING.md).
