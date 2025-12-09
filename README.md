# 🛡️ Modélisation et Audit : Registre Sécurisé des Mots de Passe Administrateurs

Ce projet représente la **conception et l'implémentation d'un Système d'Information (SI)** sécurisé et centralisé pour la gestion des mots de passe des comptes administrateurs. Il vise à résoudre le problème de l'insécurité et du manque de traçabilité.

| Informations du Projet | Détails |
| :--- | :--- |
| **Objectif Principal** | Fournir une solution robuste pour le stockage **chiffré** et l'**audit** des identifiants et mots de passe. |
| **Compétences Clés** | Modélisation de Données (MCD/MLD), SQL Querying, Data Governance, Audit Trail (Historisation). |
| **Outil d'Implémentation**| Microsoft Access (Base de Données Relationnelle). |

---

## 🚀 Compétences Techniques Démontrées

* **Modélisation de Données :** Maîtrise de la conception de schémas (MCD/MLD).
* **Gouvernance et Traçabilité :** Mise en place d'un système d'**historisation** pour l'audit rigoureux des modifications.
* **Sécurité Logique :** Prise en compte du stockage du mot de passe sous forme **cryptée**.

---

## 📋 Les Étapes de Conception

### 1. Dictionnaire de Données et Classification
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png.png)

### 2. Modèle Conceptuel de Données (MCD)
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png.png)

### 3. Modèle Logique de Données (MLD)
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png.png)

---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png.png)

### 2. Requête d'Audit et Traçabilité (Historisation)

* **L'Administrateur concerné (Requête 3):** Identification de l'administrateur associé à un mot de passe.
    ![Résultat de la Requête 3 montrant les administrateurs et les IDs de mots de passe](Ressources/Audit_Query_1.png.png)
* **L'Historique des Modifications (Requête 4):** Trace qui a modifié le mot de passe, son email, et la date de l'action (`Date_Modification`).
    ![Résultat de la Requête 4 montrant l'historique des modifications par administrateur](Ressources/Audit_Query_2.png.png)

---

### 📚 Documentation Complète
* [Rapport Complet du Projet de Système d'Information (PDF)](Rapport_Modelisation_Audit_MotsDePasse.pdf)

---


