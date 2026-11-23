
# mlops-ml-project — baseline ML reproductible

## Installation

Créer et activer l'environnement virtuel :

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Installer les dépendances :

```bash
pip install -r requirements.txt
```

## Entraînement

```bash
python scripts/train.py
```

## Évaluation

```bash
python scripts/evaluate.py
```

## Tests

```bash
python -m pytest -q
```

## Artefacts (générés dans artifacts/, non versionnés)

- `model.joblib` : pipeline entraîné (prétraitement + modèle).
- `metrics.json` : accuracy et f1_macro sur le jeu de test.
- `confusion_matrix.png` : matrice de confusion.
- `report.json` : rapport de classification détaillé.
