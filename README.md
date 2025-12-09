# Modelisation-Audit-Registre-Mdp-Admin
Conception et implémentation d'un Système d'Information sécurisé pour le Registre des Mots de Passe Administrateurs, mettant en avant les compétences en modélisation de données (MCD/MLD) et en traçabilité (Audit Trail).

# 🛡️ Modélisation et Audit : Registre Sécurisé des Mots de Passe Administrateurs

Ce projet représente la **conception et l'implémentation d'un Système d'Information (SI)** sécurisé pour la gestion des mots de passe des comptes administrateurs. [cite_start]Il vise à résoudre le problème de l'insécurité et du manque de traçabilité en mettant l'accent sur la **modélisation des données** et la **gouvernance**. [cite: 425, 426]

| Informations du Projet | Détails |
| :--- | :--- |
| **Objectif Principal** | [cite_start]Fournir une solution robuste pour le stockage **chiffré** et l'**audit** des identifiants et mots de passe. [cite: 426] |
| **Compétences Clés** | Modélisation de Données (MCD/MLD), SQL Querying, Data Governance, Audit Trail (Historisation). |
| **Outil d'Implémentation**| Microsoft Access (Base de Données Relationnelle). |

---

## 🚀 Compétences Techniques Démontrées (Data Modeling & Governance)

Ce projet valorise les compétences fondamentales d'un **Data Analyst / Modeler** :

* [cite_start]**Modélisation de Données :** Maîtrise de la conception de schémas (MCD/MLD) pour créer une structure de données optimisée. [cite: 419, 463, 520]
* [cite_start]**Gouvernance et Traçabilité :** Définition du **dictionnaire de données** et mise en place d'un système d'**historisation** pour l'audit rigoureux des modifications. [cite: 436, 431]
* [cite_start]**Sécurité Logique :** Prise en compte du stockage du mot de passe sous forme **cryptée** (via l'attribut `Mot_Passe_Crypte`). [cite: 429, 482]

---

## 📋 Les Étapes de Conception (Focus Data Architecture)

### 1. Dictionnaire de Données et Classification

[cite_start]Le dictionnaire établit la nature de chaque donnée (quantitative/qualitative, permanente/temporaire), essentielle pour la qualité et la gouvernance. [cite: 436, 437]
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png)

### 2. Modèle Conceptuel de Données (MCD)

[cite_start]Le MCD définit les entités principales du système et les **règles de gestion** via les cardinalités. [cite: 463]
* [cite_start]Il établit la relation où un mot de passe est obligatoirement (1,1) assigné à un administrateur[cite: 509].
* [cite_start]Il montre l'entité `HistoriqueMdp` pour la traçabilité des modifications[cite: 499, 431].
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png) 
### 3. Modèle Logique de Données (MLD)

[cite_start]Le MLD est la traduction du MCD en structure de tables (`ADMINISTRATEUR`, `MOTDEPASSE`, `SYSTEME`, `HISTORIQUEMDP`), définissant les clés primaires et étrangères. [cite: 520]
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png) 
---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)

[cite_start]Ce schéma montre la mise en œuvre effective des relations (définies dans le MLD) au sein de Microsoft Access, garantissant l'**intégrité référentielle** de la base de données. [cite: 807]
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png) 
### 2. Requête d'Audit et Traçabilité (Historisation)

[cite_start]Ces requêtes démontrent la capacité d'**extraction de données (SQL Querying)** et d'**audit** (page 13 du rapport)[cite: 419, 809].

* **L'Administrateur concerné (Requête 3):** Identification de l'administrateur associé à un mot de passe.
    ![Résultat de la Requête 3 montrant les administrateurs et les IDs de mots de passe](Ressources/Audit_Query_1.png) * **L'Historique des Modifications (Requête 4):** Trace qui a modifié le mot de passe, son email, et la date de l'action (`Date_Modification`).
    ![Résultat de la Requête 4 montrant l'historique des modifications par administrateur](Ressources/Audit_Query_2.png) 
---

### 📚 Documentation Complète

[cite_start]Pour une analyse détaillée (création de tables, formulaires [cite: 811][cite_start], requêtes complètes, états [cite: 813]), veuillez consulter le rapport académique complet :
* [Rapport Complet du Projet de Système d'Information (PDF)](Documentation/Rapport_Modelisation_Audit_MotsDePasse.pdf)
