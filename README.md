# Modelisation-Audit-Registre-Mdp-Admin
Conception et implémentation d'un Système d'Information sécurisé pour le Registre des Mots de Passe Administrateurs, mettant en avant les compétences en modélisation de données (MCD/MLD) et en traçabilité (Audit Trail).

# 🛡️ Modélisation et Audit : Registre Sécurisé des Mots de Passe Administrateurs

[cite_start]Ce projet représente la **conception et l'implémentation d'un Système d'Information (SI)** sécurisé pour la gestion des mots de passe des comptes administrateurs[cite: 18]. [cite_start]Il vise à résoudre le problème de l'insécurité et du manque de traçabilité en mettant l'accent sur la **modélisation des données** et la **gouvernance**[cite: 19].

| Informations du Projet | Détails |
| :--- | :--- |
| **Objectif Principal** | [cite_start]Fournir une solution robuste pour le stockage **chiffré** et l'**audit** des identifiants et mots de passe[cite: 19]. |
| **Compétences Clés** | [cite_start]Modélisation de Données (MCD/MLD), SQL Querying, Data Governance, Audit Trail (Historisation)[cite: 19, 24]. |
| **Outil d'Implémentation**| Microsoft Access (Base de Données Relationnelle). |

---

## 🚀 Compétences Techniques Démontrées (Data Modeling & Governance)

Ce projet valorise les compétences fondamentales d'un **Data Analyst / Modeler** :

* [cite_start]**Modélisation de Données :** Maîtrise de la conception de schémas (MCD/MLD) pour créer une structure de données optimisée[cite: 56, 113].
* [cite_start]**Gouvernance et Traçabilité :** Mise en place d'un système d'**historisation** pour l'audit rigoureux des modifications[cite: 24, 107].
* [cite_start]**Sécurité Logique :** Prise en compte du stockage du mot de passe sous forme **cryptée**[cite: 19, 22].

---

## 📋 Les Étapes de Conception (Focus Data Architecture)

### 1. Dictionnaire de Données et Classification

[cite_start]Le dictionnaire (page 4 du rapport) établit la nature de chaque donnée (quantitative/qualitative, permanente/temporaire), essentielle pour la qualité et la gouvernance[cite: 29, 30].
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png)

### 2. Modèle Conceptuel de Données (MCD)

[cite_start]Le MCD (page 6 du rapport) définit les entités principales (`Administrateur`, `MotDePasse`, `HistoriqueMdp`) et les **règles de gestion** via les cardinalités[cite: 56].
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png) 

### 3. Modèle Logique de Données (MLD)

[cite_start]Le MLD (page 8 du rapport) est la traduction du MCD en structure de tables, définissant les clés primaires et étrangères pour l'implémentation physique[cite: 113].
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png) 

---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)

[cite_start]Ce schéma (page 11 du rapport) montre la mise en œuvre effective des relations définies dans le MLD au sein de Microsoft Access[cite: 400].
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png) 

### 2. Requête d'Audit et Traçabilité (Historisation)

[cite_start]Ces requêtes (page 13 du rapport) démontrent la capacité d'**extraction de données (SQL Querying)** et d'**audit**[cite: 402].

* [cite_start]**L'Administrateur concerné (Requête 3):** Identification de l'administrateur associé à un mot de passe[cite: 402].
    ![Résultat de la Requête 3 montrant les administrateurs et les IDs de mots de passe](Ressources/Audit_Query_1.png) 
* [cite_start]**L'Historique des Modifications (Requête 4):** Trace qui a modifié le mot de passe, son email, et la date de l'action (`Date_Modification`)[cite: 402].
    ![Résultat de la Requête 4 montrant l'historique des modifications par administrateur](Ressources/Audit_Query_2.png) 

---

### 📚 Documentation Complète (Lien Corrigé)

Pour une analyse détaillée des fonctionnalités, veuillez consulter le rapport académique complet (pages 9 à 17) :
* [Rapport Complet du Projet de Système d'Information (PDF)](Rapport_Modelisation_Audit_MotsDePasse.pdf)

---

**Khoulassa:**

1.  **Vérifiez 100%** que les images dans `Ressources/` ont les noms exacts: `Data_Dictionary.png`, `MCD_Schema.png`, `Audit_Query_1.png`, etc.
2.  **Copiez-collez** le `README.md` ci-dessus.
3.  **Actualisez** la page GitHub avec `Ctrl + F5` (ou `Cmd + R` sur Mac).
