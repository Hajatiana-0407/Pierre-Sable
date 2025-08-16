# 🏗️ Cahier des Charges – Logiciel de Gestion d’une Entreprise de Matériaux de Construction

## 📌 1. Présentation du projet
- **Nom de l’entreprise :** À compléter  
- **Activité principale :** Production et vente de matériaux de construction (sable, gravillons, mallons, pavés, etc.)  
- **Technologie utilisée :**  
  - **Langage :** Python  
  - **Framework :** Django  
  - **Base de données :** PostgreSQL (recommandé) ou MySQL  
  - **Frontend :** Django Template ou API REST + React/Vue.js (optionnel)  

---

## 🎯 2. Objectifs du logiciel
- Gérer séparément les **stocks du magasin** et de la **carrière**.  
- Enregistrer les ventes effectuées au magasin et directement à la carrière.  
- Gérer les **transferts internes** (carrière → magasin) avec ajout des **frais de transport**.  
- Gérer les **produits avec unité de mesure** (m³, tonne, pièce, sac, etc.).  
- Gérer le personnel et calculer automatiquement les **rémunérations mensuelles**.  
- Automatiser la **facturation, les paiements et les crédits**.  
- Fournir des **rapports statistiques et financiers**.  

---

## ⚙️ 3. Fonctionnalités principales

### 📦 3.1. Gestion des produits
- Ajouter, modifier, supprimer des produits.  
- Définir une **unité de mesure** pour chaque produit.  
- Exemples d’unités :  

| Produit       | Unité de mesure |
|---------------|-----------------|
| Sable         | m³              |
| Gravillons    | tonne           |
| Mallons       | pièce           |
| Pavés         | pièce           |

---

### 🏭 3.2. Gestion des stocks
- **Stock carrière :** matériaux produits sur place.  
- **Stock magasin :** matériaux disponibles pour la vente au public.  
- **Mouvements internes :** transfert carrière → magasin avec ajout du **coût de transport** (camion, carburant, chauffeur).  
- Alerte stock faible.  

---

### 💰 3.3. Gestion des ventes
- **Ventes magasin :** clients du point de vente.  
- **Ventes carrière :** clients achetant directement à la carrière.  
- Génération de **factures et bons de commande**.  
- Suivi des paiements : espèces, mobile money, virement, crédit.  
- Historique par client.  

---

### ⚒️ 3.4. Gestion de la production (carrière)
- Enregistrement de la **production journalière** par type de produit.  
- Déduction automatique du stock lors des ventes sur place.  
- Statistiques de productivité.  

---

### 🚚 3.5. Gestion des approvisionnements internes
- Création d’un **bon de transfert** (carrière → magasin).  
- Ajout du **frais de transport** au prix de revient.  
- Historique des transferts.  

---

### 👷 3.6. Gestion du personnel et salaires
- **Carrière :** ouvriers de production (tailleurs de mallons, concasseurs, etc.).  
- **Magasin :** vendeuses, caissières, chargeurs de camions.  
- Fiche employé : (Nom, fonction, salaire de base, jours/heures travaillés).  
- Calcul automatique du **salaire mensuel** (fixe + primes éventuelles).  
- Gestion des **avances sur salaire**.  

---

### 📊 3.7. Comptabilité et rapports
- Suivi des **recettes et dépenses**.  
- Intégration des **frais de transport** et du **coût de production** dans les prix de revient.  
- Rapports disponibles :  
  - Stock (carrière et magasin séparés)  
  - Ventes (par produit, par site, par client)  
  - Production journalière/mensuelle  
  - Approvisionnements internes  
  - Paie du personnel  
  - Bilan et résultats mensuels  

---

## 👥 4. Utilisateurs du système
- **Administrateur :** accès complet  
- **Responsable carrière :** production + ventes carrière  
- **Magasinier :** gestion stock magasin + ventes  
- **Caissier/Vendeuse :** encaissements et factures  
- **Comptable :** finances et salaires  

---

## 🔒 5. Sécurité
- Gestion des rôles et permissions.  
- Historique des actions (traçabilité).  
- Sauvegarde régulière de la base de données.  

---

## ⏳ 6. Délais et budget
- **Durée estimée :** 4 à 6 mois de développement.  
- **Budget :** à définir selon équipe et fonctionnalités supplémentaires.  

---

## 🚀 7. Évolutions futures possibles
- Module RH complet (congés, absences, primes).  
- Application mobile (commandes clients en ligne).  
- Intégration de facturation électronique.  
- Suivi GPS des camions de transport.  
