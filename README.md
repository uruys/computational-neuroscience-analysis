# computational-neuroscience-analysis
Analyse computationnelle de données neurophysiologiques et comportementales utilisant Python (NumPy, Pandas, Matplotlib, DeepLabCut). Inclut le traitement du signal, l’analyse du mouvement et la visualisation de données appliquées aux neurosciences.

# Computational Neuroscience Data Analysis (DeepLabCut)

Ce repository contient un pipeline d’analyse computationnelle de données comportementales et neurophysiologiques basé sur DeepLabCut et Python. Il reproduit un workflow utilisé en recherche en neurosciences pour le suivi et l’analyse cinématique des mouvements chez la souris.

## Contexte scientifique

Ce projet s’inscrit dans un contexte de recherche en neurosciences computationnelles impliquant :

- Tracking automatisé de points anatomiques avec DeepLabCut
- Extraction des coordonnées (x, y) de différentes parties du corps
- Analyse des trajectoires et de la cinématique du mouvement
- Traitement et visualisation de données comportementales

Ce travail est basé sur une expérience de stage en laboratoire de neurosciences (NeuroPSI, CNRS / Université Paris-Saclay), impliquant l’analyse de données comportementales et neurophysiologiques.

## Objectifs

Le pipeline permet de :

- Charger des données DeepLabCut (CSV MultiIndex)
- Filtrer les données selon le score de confiance (likelihood, p-cutoff)
- Nettoyer les artefacts et interpoler les données manquantes
- Calculer des métriques cinématiques :
  - trajectoires
  - vitesse
  - distance parcourue
- Générer des visualisations scientifiques des mouvements

## Technologies utilisées

- Python
- NumPy
- Pandas
- Matplotlib
- DeepLabCut (sorties CSV)

## Exemple d’utilisation

Installer les dépendances :

```bash
pip install -r requirements.txt

python src/dlc_kinematics.py --csv data/exemple_dlc.csv --out figures
