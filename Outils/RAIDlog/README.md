# ✅ **RAID Log – Explication (AgilePM v3)**

Le **RAID Log** est un outil essentiel de gestion de projet qui permet de **centraliser et suivre** quatre catégories critiques :

**R – Risks (Risques)**
Événements potentiels susceptibles d’avoir un impact négatif sur le projet. On y note : description, probabilité, impact, propriétaire, actions d’atténuation.

**A – Assumptions (Hypothèses)**
Éléments considérés comme vrais pour planifier le projet, mais non encore prouvés. Elles doivent être validées régulièrement.

**I – Issues (Problèmes / Incidents)**
Événements déjà survenus et qui affectent réellement le projet. Ils nécessitent une action immédiate.

**D – Dependencies (Dépendances)**
Relations ou conditions nécessaires avant d’avancer (internes ou externes).
Ex : dépendance avec un fournisseur, une équipe, ou une livraison technique.

---

## 🎯 **Pourquoi utiliser un RAID Log dans AgilePM v3 ?**

* Permet une **visibilité claire et partagée** de ce qui peut menacer la livraison.
* Soutient la logique AgilePM : **prévisibilité, transparence et gestion proactive**.
* Aide le **Project Manager, Business Sponsor et Team Leader** à prendre de bonnes décisions.
* Favorise l’apprentissage continu : le RAID Log est mis à jour **à chaque timebox**, **SAD**, **Foundations**, **Delivery Planning**, etc.

---

# 📘 **Exemple 1 – RAID Log (Projet : Déploiement portail client)**

### **Risks (Risques)**

| ID | Description           | Impact | Probabilité | Score | Propriétaire | Plan d’action                                  |
| -- | --------------------- | ------ | ----------- | ----- | ------------ | ---------------------------------------------- |
| R1 | Retard de l’équipe UX | Moyen  | Élevé       | 12    | Team Leader  | Ajouter un UX backup + réduire scope Must Have |

### **Assumptions (Hypothèses)**

| ID | Hypothèse                                  | Validité    | Propriétaire     | Date de revue   |
| -- | ------------------------------------------ | ----------- | ---------------- | --------------- |
| A1 | Les données clients sont propres et à jour | À confirmer | Business Analyst | Fin du Sprint 1 |

### **Issues (Problèmes)**

| ID | Problème               | Impact | Statut   | Propriétaire | Actions                                |
| -- | ---------------------- | ------ | -------- | ------------ | -------------------------------------- |
| I1 | API Auth ne répond pas | Fort   | En cours | Dev Lead     | Analyse logs + escalade à l’équipe IAM |

### **Dependencies (Dépendances)**

| ID | Dépendance                      | Type          | Statut     | Responsable   | Échéance |
| -- | ------------------------------- | ------------- | ---------- | ------------- | -------- |
| D1 | Livraison du module facturation | Externe (ERP) | En attente | Architecte SI | 10/12    |

---

# 📙 **Exemple 2 – RAID Log (Projet : Migration infrastructure Cloud)**

### **Risks**

| ID | Description                           | Impact | Prob  | Score | Owner             | Mitigation                           |
| -- | ------------------------------------- | ------ | ----- | ----- | ----------------- | ------------------------------------ |
| R2 | Surcharge réseau lors de la migration | Élevé  | Moyen | 9     | Architecte Réseau | Plan migration nocturne + monitoring |

### **Assumptions**

| ID | Hypothèse                            | Validité | Owner   | Review      |
| -- | ------------------------------------ | -------- | ------- | ----------- |
| A2 | Le budget supplémentaire sera validé | Risqué   | Sponsor | Revue hebdo |

### **Issues**

| ID | Problème                    | Impact | Statut   | Owner | Action               |
| -- | --------------------------- | ------ | -------- | ----- | -------------------- |
| I2 | Manque de licences firewall | Élevé  | Bloquant | PM    | Commander en urgence |

### **Dependencies**

| ID | Dépendance                            | Type    | Statut     | Owner      | Due   |
| -- | ------------------------------------- | ------- | ---------- | ---------- | ----- |
| D2 | Validation juridique pour stockage UE | Externe | En analyse | Compliance | 05/01 |

---

# 📗 **Exemple 3 – RAID Log (Projet : Développement application mobile IoT Smart Meter)**

### **Risks**

| ID | Description                                    | Impact | Prob  | Score | Owner         | Mitigation                         |
| -- | ---------------------------------------------- | ------ | ----- | ----- | ------------- | ---------------------------------- |
| R3 | Instabilité du réseau GSM dans certaines zones | Moyen  | Élevé | 12    | Product Owner | Prévoir mode offline + cache local |

### **Assumptions**

| ID | Hypothèse                                  | Validité   | Owner         | Review   |
| -- | ------------------------------------------ | ---------- | ------------- | -------- |
| A3 | Les compteurs IoT en place supportent MQTT | À vérifier | Tech Lead IoT | Sprint 2 |

### **Issues**

| ID | Problème                      | Impact     | Statut | Owner    | Action                           |
| -- | ----------------------------- | ---------- | ------ | -------- | -------------------------------- |
| I3 | Bug critique sur firmware 1.2 | Très élevé | Ouvert | Team IoT | Rollback vers version stable 1.1 |

### **Dependencies**

| ID | Dépendance                      | Type    | Statut     | Owner              | Deadline |
| -- | ------------------------------- | ------- | ---------- | ------------------ | -------- |
| D3 | Livraison clé API du régulateur | Externe | En attente | Responsable métier | 20/12    |

---

