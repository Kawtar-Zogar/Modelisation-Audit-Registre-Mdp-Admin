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

## 📋 Les Étapes de Conception (Focus Data Architecture)

### 1. Dictionnaire de Données et Classification
**Chra7:** Hada howa l-jadwal l'awal (page 4), kaywerri kolla **donnée** (b7al `ID Admin`, `Nom Admin`, `Mot_Passe_Crypte`), w kay7addad l-format dyalha w l-classification (Quantitative/Qualitative, Permanente/Temporaire). Hada mouhim l'l'**Gouvernance** w **Qualité des Données**.
![Tableau du Dictionnaire de Données montrant la classification](Ressources/Data_Dictionary.png.png)

### 2. Modèle Conceptuel de Données (MCD)
**Chra7:** L-MCD (page 6) howa l-khalita dial l'3ala9at bin l-Entités l-Asasiya (b7al `Administrateur`, `MotDePasse`, `HistoriqueMdp`). Kaywerri **l-règles dial l-gestion** (b7al: koll **`MotDePasse`** khasso ykoun **`assigné`** l'wa7ed **`Administrateur`**).
![Modèle Conceptuel de Données (MCD) du registre de mots de passe](Ressources/MCD_Schema.png.png)

### 3. Modèle Logique de Données (MLD)
**Chra7:** L-MLD (page 8) howa tarjama dial l-MCD l'wa7ed l-structure dial les tables (`ADMINISTRATEUR`, `MOTDEPASSE`, `SYSTEME`, `HISTORIQUEMDP`), m3a l-Clés Primaires (PK) w l-Clés Étrangères (FK). Hada howa l'design li ghandirou bih l-Base de Données f'Access.
![Modèle Logique de Données (MLD) du registre de mots de passe](Ressources/MLD_Schema.png.png)

---

## 🛠️ Implémentation et Exploitation (SQL et Audit)

### 1. Relations entre les Tables (Intégrité Référentielle)
**Chra7:** Had l'image (page 11) katchra7 kifach l-Tables tconnktao (li howa tarjama dial l-MLD) f'l-Logiciel **MS Access**. Had l'connexion mouhima bach n'dmennou l'**Intégrité Référentielle** (ma t9derch t7eddef wa7ed l'Administrateur bla ma t'sawweb l'Mots de Passe dialou l'lawlin).
![Schéma des relations entre les tables dans Access](Ressources/Relations_Access.png.png)

### 2. Requête d'Audit et Traçabilité (Historisation)

Had les requêtes kaywerriwna l'9odra dial l-Système 3la l'**Traçabilité** w l'**Audit** (page 13):

* **L'Administrateur concerné (Requête 3):**
    **Chra7:** Had l'requête katsta3mel l'SQL bach t'extracti **smiyat l-Administrateurs** m3a l'ID dial l-Mots de Passe li m'assinyin lihom. Katchra7 chkoun responsable 3la achmen compte.
    ![Résultat de la Requête 3 montrant les administrateurs et les IDs de mots de passe](Ressources/Audit_Query_1.png.png)

* **L'Historique des Modifications (Requête 4):**
    **Chra7:** Had l'requête katchouf table **`HistoriqueMdp`**. Katwerri **chkoune** (par `Nom_Admin` w `Email_Admin`) **wa9tach** (`Date_Modification`) b'ddabt dar l-tghyir 3la wa7ed l-mot de passe. Hada howa l'Audit Trail l'Moussa77a7.
    ![Résultat de la Requête 4 montrant l'historique des modifications par administrateur](Ressources/Audit_Query_2.png.png)

---

### 📚 Documentation Complète
* [Rapport Complet du Projet de Système d'Information (PDF)](Rapport_Modelisation_Audit_MotsDePasse.pdf)

---
