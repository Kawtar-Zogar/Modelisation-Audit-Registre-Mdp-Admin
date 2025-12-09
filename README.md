# Modelisation-Audit-Registre-Mdp-Admin
Conception et implémentation d'un Système d'Information sécurisé pour le Registre des Mots de Passe Administrateurs, mettant en avant les compétences en modélisation de données (MCD/MLD) et en traçabilité (Audit Trail).

# 🛡️ Modélisation et Audit : Registre Sécurisé des Mots de Passe Administrateurs

Ce projet représente la **conception et l'implémentation d'un Système d'Information (SI)** sécurisé pour la gestion des mots de passe des comptes administrateurs.

---

## 🚀 Compétences Techniques Démontrées

* **Modélisation de Données :** Maîtrise de la conception de schémas (MCD/MLD).
* **Gouvernance et Traçabilité :** Mise en place d'un système d'**historisation** pour l'audit rigoureux des modifications.
* **Sécurité Logique :** Prise en compte du stockage du mot de passe sous forme **cryptée**.

---

## 📋 Les Étapes de Conception

### 1. Dictionnaire de Données et Classification
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png)

### 2. Modèle Conceptuel de Données (MCD)
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png) 
### 3. Modèle Logique de Données (MLD)
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png) 
---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png) 
### 2. Requête d'Audit et Traçabilité (Historisation)

* **L'Administrateur concerné (Requête 3):** Identification de l'administrateur associé à un mot de passe.
    ![Résultat de la Requête 3 montrant les administrateurs et les IDs de mots de passe](Ressources/Audit_Query_1.png) * **L'Historique des Modifications (Requête 4):** Trace qui a modifié le mot de passe, son email, et la date de l'action (`Date_Modification`).
    ![Résultat de la Requête 4 montrant l'historique des modifications par administrateur](Ressources/Audit_Query_2.png) 
---

### 📚 Documentation Complète
* [Rapport Complet du Projet de Système d'Information (PDF)](Rapport_Modelisation_Audit_MotsDePasse.pdf)
