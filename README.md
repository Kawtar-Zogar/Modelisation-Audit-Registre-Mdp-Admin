# Modelisation-Audit-Registre-Mdp-Admin
Conception et implémentation d'un Système d'Information sécurisé pour le Registre des Mots de Passe Administrateurs, mettant en avant les compétences en modélisation de données (MCD/MLD) et en traçabilité (Audit Trail).

# 🛡️ Modélisation et Audit : Registre Sécurisé des Mots de Passe Administrateurs

Ce projet représente la **conception et l'implémentation d'un Système d'Information (SI)** sécurisé pour la gestion des mots de passe des comptes administrateurs. Il vise à résoudre le problème de l'insécurité et du manque de traçabilité en mettant l'accent sur la **modélisation des données** et la **gouvernance**.

| Informations du Projet | Détails |
| :--- | :--- |
| **Objectif Principal** | Fournir une solution robuste pour le stockage **chiffré** et l'**audit** des identifiants et mots de passe. |
| **Compétences Clés** | Modélisation de Données (MCD/MLD), SQL Querying, Data Governance, Audit Trail (Historisation). |
| **Outil d'Implémentation**| Microsoft Access (Base de Données Relationnelle). |

---

## 🚀 Compétences Techniques Démontrées (Data Modeling & Governance)

Ce projet valorise les compétences fondamentales d'un **Data Analyst / Modeler** :

* **Modélisation de Données :** Maîtrise de la conception de schémas (MCD/MLD) pour créer une structure de données optimisée.
* **Gouvernance et Traçabilité :** Définition du dictionnaire de données et mise en place d'un système d'**historisation** pour l'audit rigoureux des modifications.
* **Sécurité Logique :** Prise en compte du stockage du mot de passe sous forme **cryptée** (via l'attribut `Mot_Passe_Crypte`).

---

## 📋 Les Étapes de Conception (Focus Data Architecture)

### 1. Dictionnaire de Données et Classification

Le dictionnaire (page 4 du rapport) établit la nature de chaque donnée (quantitative/qualitative, permanente/temporaire), essentielle pour la qualité et la gouvernance.
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png)

### 2. Modèle Conceptuel de Données (MCD)

Le MCD (page 6 du rapport) définit les entités principales du système et les **règles de gestion** via les cardinalités.
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png) 

### 3. Modèle Logique de Données (MLD)

Le MLD (page 8 du rapport) est la traduction du MCD en structure de tables, définissant les clés primaires et étrangères pour l'implémentation physique.
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png) 

---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)

Ce schéma (page 11 du rapport) montre la mise en œuvre effective des relations définies dans le MLD au sein de Microsoft Access, garantissant l'**intégrité référentielle** de la base de données.
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png) 

### 2. Requête d'Audit et Traçabilité (Query 4)

Cette requête (page 13 du rapport) démontre la capacité d'**extraction de données (SQL Querying)** et d'**audit**. Elle permet de tracer :

* **L'Administrateur concerné (Query 3):** Qui a des mots de passe dans le registre.
    ![Résultat de la Requête 3 montrant les administrateurs et les IDs de mots de passe](Ressources/Audit_Query_1.png) 
* **L'Historique des Modifications (Query 4):** Qui (`Nom_Admin`) a effectué la modification, son email, et la date de l'action (`Date_Modification`).
    ![Résultat de la Requête 4 montrant l'historique des modifications par administrateur](Ressources/Audit_Query_2.png) 

---

### 📚 Documentation Complète

Pour une analyse détaillée des fonctionnalités (création de tables, formulaires, requêtes complètes, états), veuillez consulter le rapport académique complet :
* [Rapport Complet du Projet de Système d'Information (PDF)](Documentation/Rapport_Modelisation_Audit_MotsDePasse.pdf)
