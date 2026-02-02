# 📊 Gantt Generic - Générateur de Diagrammes de Gantt

Application Streamlit générique pour créer des diagrammes de Gantt à partir de fichiers Excel ou CSV.

**Différence avec gantt_generator_V1/V2** : Cette version utilise des colonnes génériques (catégorie, tâche, début, fin) au lieu des colonnes spécifiques aux modèles murins.

## 🚀 Démo en ligne

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://sandrine-crypto-gantt-generator.streamlit.app)

## 📋 Colonnes requises

Votre fichier doit contenir les colonnes suivantes :

| Colonne | Description | Exemple |
|---------|-------------|---------|
| `catégorie` | Groupe ou phase du projet | "Phase 1", "Développement" |
| `tâche` | Nom de la tâche | "Analyse des besoins" |
| `début` | Date de début | 2025-01-15 |
| `fin` | Date de fin | 2025-02-28 |

### Noms de colonnes acceptés

L'application reconnaît automatiquement plusieurs variantes :
- **Catégorie** : `catégorie`, `categorie`, `category`, `groupe`, `group`
- **Tâche** : `tâche`, `tache`, `task`, `nom`, `name`, `activité`
- **Début** : `début`, `debut`, `start`, `date_debut`, `start_date`
- **Fin** : `fin`, `end`, `date_fin`, `end_date`, `échéance`

### Formats de date acceptés

- `YYYY-MM-DD` (2025-01-15)
- `DD/MM/YYYY` (15/01/2025)
- `DD-MM-YYYY` (15-01-2025)
- `DD.MM.YYYY` (15.01.2025)

## ✨ Fonctionnalités

- ✅ Upload de fichiers Excel (.xlsx) et CSV
- ✅ Détection automatique des colonnes
- ✅ Vue globale ou par catégorie
- ✅ Diagrammes SVG interactifs avec tooltips
- ✅ Export CSV des données traitées
- ✅ Export SVG du diagramme
- ✅ Export rapport HTML complet (multi-pages)
- ✅ Template téléchargeable

## 🛠️ Installation locale

```bash
# Cloner le dépôt
git clone https://github.com/sandrine-crypto/Gantt-generator.git
cd Gantt-generator

# Installer les dépendances
pip install -r requirements.txt

# Lancer l'application
streamlit run gantt_generic.py
```

## 📁 Structure du projet

```
Gantt-generator/
├── gantt_generic.py      # Application Streamlit générique (colonnes: catégorie, tâche, début, fin)
├── gantt_generator_V1.py # Script original V1 (modèles murins)
├── gantt_generator_V2.py # Script original V2 (modèles murins)
├── requirements.txt      # Dépendances Python
└── README.md            # Documentation
```

## 📊 Exemple de fichier Excel

| catégorie | tâche | début | fin |
|-----------|-------|-------|-----|
| Phase 1 | Analyse | 2025-01-01 | 2025-01-14 |
| Phase 1 | Conception | 2025-01-15 | 2025-01-31 |
| Phase 2 | Développement | 2025-02-01 | 2025-03-15 |
| Phase 2 | Tests | 2025-03-01 | 2025-03-31 |
| Phase 3 | Déploiement | 2025-04-01 | 2025-04-15 |

## 🚀 Déploiement sur Streamlit Cloud

1. Connectez-vous sur [share.streamlit.io](https://share.streamlit.io)
2. Cliquez sur "New app"
3. Sélectionnez le dépôt `sandrine-crypto/Gantt-generator`
4. **Main file path** : `gantt_generic.py`
5. Cliquez sur "Deploy"

## 📝 Licence

Usage interne - CRUPPE

## 📧 Contact

**Développement:** CRUPPE - Biologie Moléculaire  
**Localisation:** Lyon, Rhône-Alpes
