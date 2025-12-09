# Modelisation-Audit-Registre-Mdp-Admin
Conception et implémentation d'un Système d'Information sécurisé pour le Registre des Mots de Passe Administrateurs, mettant en avant les compétences en modélisation de données (MCD/MLD) et en traçabilité (Audit Trail).

# 🛡️ Modélisation et Audit : Registre Sécurisé des Mots de Passe Administrateurs

Ce projet représente la **conception et l'implémentation d'un Système d'Information (SI)** sécurisé pour la gestion des mots de passe des comptes administrateurs. [cite_start]Il vise à résoudre le problème de l'insécurité et du manque de traçabilité [cite: 16, 17] en mettant l'accent sur la **modélisation des données** et la **gouvernance**.

| Informations du Projet | Détails |
| :--- | :--- |
| **Objectif Principal** | [cite_start]Fournir une solution robuste pour le stockage **chiffré** et l'**audit** des identifiants et mots de passe[cite: 18, 19]. |
| **Compétences Clés** | Modélisation de Données (MCD/MLD), SQL Querying, Data Governance, Audit Trail. |
| **Outil d'Implémentation**| Microsoft Access (Base de Données Relationnelle). |

---

## 🚀 Compétences Techniques Démontrées (Data Modeling & Governance)

Ce projet valorise les compétences fondamentales d'un **Data Analyst / Modeler** :

* [cite_start]**Modélisation de Données :** Maîtrise de la conception de schémas (MCD/MLD) pour organiser efficacement les données sensibles[cite: 12].
* [cite_start]**Gouvernance et Traçabilité :** Définition du dictionnaire de données et mise en place d'un système d'**historisation** pour l'audit rigoureux des modifications[cite: 24, 29].
* [cite_start]**Sécurité des Données :** Prise en compte du stockage du mot de passe sous forme **cryptée**[cite: 19].

---

## 📋 Les Étapes de Conception (Focus Data Architecture)

### 1. Dictionnaire de Données et Classification

[cite_start]Le dictionnaire (page 4 du rapport) définit la nature de chaque donnée (quantitative/qualitative, permanente/temporaire)[cite: 30], essentielle pour la qualité et la gouvernance.
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png)

### 2. Modèle Conceptuel de Données (MCD)

[cite_start]Le MCD (page 6 du rapport) définit les entités principales (`Administrateur`, `MotDePasse`, `Système`, `HistoriqueMdp`) et les **règles de gestion** via les cardinalités[cite: 56]. [cite_start]Il montre notamment la relation d'**Historisation** et d'**Affectation** des mots de passe[cite: 106, 100].
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png) 
### 3. Modèle Logique de Données (MLD)

[cite_start]Le MLD (page 8 du rapport) est la traduction du MCD en structure de tables, définissant les clés primaires et étrangères pour l'implémentation physique[cite: 113].
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png) 
---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)

Ce schéma (page 11 du rapport) montre la mise en œuvre effective des relations définies dans le MLD au sein de Microsoft Access, garantissant l'**intégrité référentielle** de la base de données.
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png) 
### 2. Requête d'Audit et Traçabilité

Cette requête (page 13 du rapport) démontre la capacité d'**extraction de données (SQL Querying)** et d'**audit**. [cite_start]Elle permet de tracer qui (`Nom Admin`) a modifié un mot de passe et à quelle date (`Date Modification`), un pilier de la gouvernance de données[cite: 24, 368].
![Résultat de la Requête d'Audit montrant l'administrateur et la date de modification](Ressources/Audit_Query.png) 
---

### 📚 Documentation Complète

Pour une analyse détaillée des fonctionnalités (création de tables, formulaires, requêtes complètes, états), veuillez consulter le rapport académique complet (pages 9 à 17) :
* [Rapport Complet du Projet de Système d'Information (PDF)](Documentation/Rapport_Modelisation_Audit_MotsDePasse.pdf)
