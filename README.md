# Medtech Radar

Veille automatisée du secteur medtech : collecte (n8n), stockage et détection des changements (PostgreSQL), synthèses IA et dashboard (Streamlit).

## Structure

| Dossier / fichier | Contenu |
|---|---|
| `workflows/` | Exports JSON des workflows n8n |
| `sql/` | Schéma PostgreSQL, requêtes et détection des changements |
| `data/` | Petits exemples de données autorisés ou synthétiques |
| `dashboard/` | Code Streamlit / fichiers du dashboard |
| `evaluation/` | Tests de détection et évaluation des synthèses IA |
| `docs/` | Architecture, schéma de données, décisions techniques |
| `.env.example` | Variables de configuration sans secrets |
| `.gitignore` | Exclusion des secrets et fichiers locaux |

## Reproduction

1. Copier `.env.example` vers `.env` et renseigner les valeurs.
2. Créer la base PostgreSQL et appliquer le schéma de `sql/`.
3. Importer les workflows de `workflows/` dans n8n.
4. Lancer le dashboard : `streamlit run dashboard/app.py`.

_À compléter au fil du projet._
