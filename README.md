# Modelisation-Audit-Registre-Mdp-Admin
Conception et implémentation d'un Système d'Information sécurisé pour le Registre des Mots de Passe Administrateurs, mettant en avant les compétences en modélisation de données (MCD/MLD) et en traçabilité (Audit Trail).

# 🛡️ Modélisation et Audit : Registre Sécurisé des Mots de Passe Administrateurs

[cite_start]Ce projet représente la **conception et l'implémentation d'un Système d'Information (SI)** sécurisé pour la gestion des mots de passe des comptes administrateurs[cite: 425]. [cite_start]Il vise à résoudre le problème de l'insécurité et du manque de traçabilité [cite: 424] en mettant l'accent sur la **modélisation des données** et la **gouvernance**.

| Informations du Projet | Détails |
| :--- | :--- |
| **Objectif Principal** | [cite_start]Fournir une solution robuste pour le stockage **chiffré** [cite: 429] [cite_start]et l'**audit** des identifiants et mots de passe[cite: 426]. |
| **Compétences Clés** | [cite_start]Modélisation de Données (MCD/MLD), SQL Querying, Data Governance, Audit Trail (Historisation)[cite: 431]. |
| **Outil d'Implémentation**| Microsoft Access (Base de Données Relationnelle). |

---

## 🚀 Compétences Techniques Démontrées (Data Modeling & Governance)

Ce projet valorise les compétences fondamentales d'un **Data Analyst / Modeler** :

* [cite_start]**Modélisation de Données :** Maîtrise de la conception de schémas (MCD/MLD) pour créer une structure de données optimisée[cite: 463, 520].
* [cite_start]**Gouvernance et Traçabilité :** Définition du dictionnaire de données [cite: 436] [cite_start]et mise en place d'un système d'**historisation** pour l'audit rigoureux des modifications[cite: 431].
* [cite_start]**Sécurité Logique :** Prise en compte du stockage du mot de passe sous forme **cryptée** (via l'attribut `Mot_Passe_Crypte`)[cite: 429, 437].

---

## 📋 Les Étapes de Conception (Focus Data Architecture)

### 1. Dictionnaire de Données et Classification

[cite_start]Le dictionnaire (page 4 du rapport) établit la nature de chaque donnée (quantitative/qualitative, permanente/temporaire), essentielle pour la qualité et la gouvernance[cite: 437].
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png)

### 2. Modèle Conceptuel de Données (MCD)

[cite_start]Le MCD (page 6 du rapport) définit les entités principales (`Administrateur`, `MotDePasse`, `HistoriqueMdp` [cite: 464, 495, 499][cite_start]) et les **règles de gestion** via les cardinalités (par exemple, chaque mot de passe est obligatoirement (1,1) assigné à un administrateur [cite: 509]).
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png) 
### 3. Modèle Logique de Données (MLD)

[cite_start]Le MLD (page 8 du rapport) est la traduction du MCD en structure de tables (`ADMINISTRATEUR`, `MOTDEPASSE`, `SYSTEME`, `HISTORIQUEMDP` [cite: 521, 522, 530, 539][cite_start]), définissant les clés primaires et étrangères pour l'implémentation physique[cite: 520].
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png) 
---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)

[cite_start]Ce schéma (page 11 du rapport) montre la mise en œuvre effective des relations définies dans le MLD au sein de Microsoft Access, garantissant l'**intégrité référentielle** de la base de données[cite: 807].
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png) 
### 2. Requête d'Audit et Traçabilité (Query 4)

[cite_start]Cette requête (page 13 du rapport) démontre la capacité d'**extraction de données (SQL Querying)** et d'**audit**[cite: 809]. Elle permet de tracer :

* [cite_start]**L'Administrateur concerné (Query 3):** Qui a des mots de passe dans le registre[cite: 809].
    ![Résultat de la Requête 3 montrant les administrateurs et les IDs de mots de passe](Ressources/Audit_Query_1.png) * [cite_start]**L'Historique des Modifications (Query 4):** Qui (`Nom_Admin`) a effectué la modification, son email, et la date de l'action (`Date_Modification`)[cite: 774, 775, 809].
    ![Résultat de la Requête 4 montrant l'historique des modifications par administrateur](Ressources/Audit_Query_2.png) 
---

### 📚 Documentation Complète

Pour une analyse détaillée des fonctionnalités (création de tables, formulaires, requêtes complètes, états), veuillez consulter le rapport académique complet :
* [Rapport Complet du Projet de Système d'Information (PDF)](Documentation/Rapport_Modelisation_Audit_MotsDePasse.pdf)
