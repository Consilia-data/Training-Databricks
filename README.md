# Consilia
# 🚀 Training_Databricks

**Training_Databricks** est un projet de démonstration et de formation orienté Data Engineering, construit autour de l’environnement **Databricks**. Il regroupe plusieurs notebooks illustrant les étapes clés d’un pipeline de traitement de données dans une architecture **Data Lakehouse** moderne.

---

## 📌 Objectifs

- Mettre en pratique l’**ingestion**, la **transformation** et l’**exploitation** de données structurées et semi-structurées via **Databricks**.
- Illustrer l’utilisation de **Delta Lake**, des **tables managées**, des **vues logiques** et des bonnes pratiques de traitement dans un environnement distribué.
- Poser les bases d’un référentiel de travail et de formation pour les futurs projets data de l’entreprise.

---

## 🧱 Architecture cible

Ce projet s’inscrit dans une architecture **Azure + Databricks**, avec :

- 📂 **Azure Data Lake Storage (ADLS Gen2)** : stockage de données brutes
- ⚙️ **Databricks (PySpark / SQL)** : traitement, transformation, enrichissement
- 📐 **Delta Lake** : stockage transactionnel avec gestion des métadonnées et historique
- 📊 **Power BI** *(optionnel)* : visualisation des données issues de la couche Gold

---

## 📚 Contenu des notebooks

| Dossier / Notebook       | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `ingestion/`             | Ingestion de fichiers CSV / JSON depuis ADLS ou DBFS                        |
| `bronze_to_silver/`      | Nettoyage, standardisation des schémas et enrichissement métier             |
| `silver_to_gold/`        | Agrégation, jointures et création de tables analytiques pour exposition     |
| `views/`                 | Création de **vues SQL** sur tables Delta pour faciliter la consommation    |
| `utils/` *(optionnel)*   | Fonctions utilitaires (gestion de schéma, contrôles, logging)               |

---

## ✅ Prérequis

- Un workspace **Databricks** opérationnel
- Un cluster Spark configuré (Runtime 11.3+ recommandé)
- Droits d’accès à un **Data Lake** ou à **DBFS**
- (Optionnel) Intégration avec **GitHub** et Unity Catalog

---

## 🛡️ Bonnes pratiques mises en œuvre

- Utilisation des couches **Bronze / Silver / Gold**
- Format **Delta Lake** pour tous les traitements persistés
- Séparation claire entre traitement, logique métier et exposition
- Reproductibilité et clarté du code (modularité, commentaires, noms explicites)
- Vérification des schémas avant fusion de fichiers

---

## 👥 Auteur

Projet développé par l’équipe **Consilia Data** – [GitHub: @Consilia-data](https://github.com/Consilia-data)  
📫 Contact : 
- rboudiba@consilia-data.com 
- zamara@consilia-data.com
- rsaber@consilia-data.com

---

## 📝 Licence

Ce projet est mis à disposition sous licence MIT. Voir le fichier `LICENSE` pour plus d’informations.
