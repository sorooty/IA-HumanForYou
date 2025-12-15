# IA for HumanForYou - Prédiction du Turnover

> Projet Machine Learning éthique pour prédire le départ des employés et proposer des leviers RH actionnables.

**Contexte** : CESI École d'Ingénieurs - A3 FISE INFO - Bloc Intelligence Artificielle  
**Date** : Décembre 2025  
**Équipe** : Groupe 5 - CESI Analytics

---

## Problématique

L'entreprise pharmaceutique HumanForYou (4000 employés, Inde) fait face à un taux de rotation de **15% par an** (600 départs). L'objectif est d'identifier les facteurs de départ et de proposer des actions de rétention **éthiques et transparentes**, conformes à l'AI Act 2024.

**Variable cible** : `Attrition` (0 = resté, 1 = parti en 2016)

---

## Données

| Dataset                    | Variables | Description                                                        |
|---------------------------|-----------|--------------------------------------------------------------------|
| `general_data.csv`        | 35        | Données RH (âge, genre, salaire, ancienneté, poste, etc.)         |
| `manager_survey_data.csv` | 3         | Évaluation manager (implication, performance)                      |
| `employee_survey_data.csv`| 4         | Enquête satisfaction (environnement, travail, équilibre)          |
| `in_time.csv`             | 1 + dates | Heures d’arrivée par jour (données badgeuse 2015)                 |
| `out_time.csv`            | 1 + dates | Heures de départ par jour (données badgeuse 2015)                 |


**Démarche éthique** : Exclusion variables sensibles (Age, Gender, MaritalStatus) conformément au RGPD et AI Act 2024.
