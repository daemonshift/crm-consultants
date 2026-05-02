# PRD — CRM pour Consultants Indépendants
**Product Requirements Document**  
Version 1.0 — Mai 2026  
Auteur : daemonshift

---

## 1. Résumé du projet

### Le problème
Les consultants et coachs indépendants gèrent leur activité client de manière fragmentée — contacts dans le téléphone, devis dans Word, relances dans la tête, factures dans Excel. Cette dispersion génère des pertes de temps, des oublis de relances et une vision floue de leur chiffre d'affaires.

### La solution
Un CRM minimaliste, pensé exclusivement pour les consultants indépendants. Une seule interface pour gérer ses clients, ses missions, ses relances et son chiffre d'affaires — sans la complexité des outils enterprise.

### La proposition de valeur
> "Le CRM qui disparaît quand tu n'en as pas besoin, et qui est là quand tu en as besoin."

---

## 2. Utilisateur cible

### Persona principal — Le consultant indépendant
- **Âge :** 28 à 45 ans
- **Statut :** Freelance ou micro-entreprise, 1 à 5 clients actifs simultanément
- **Revenus :** 3 000 à 8 000 €/mois
- **Outils actuels :** Gmail, WhatsApp, Notion, Excel, Google Calendar
- **Douleurs principales :**
  - Oublie de relancer des prospects
  - Ne sait pas combien il va gagner le mois prochain
  - Perd du temps à chercher les infos d'un client
  - Jongle entre 4 à 6 outils différents
  - Les gros CRM (HubSpot, Salesforce) sont trop complexes et trop chers

---

## 3. Étude de marché

### Problèmes validés par la recherche
D'après l'analyse du marché 2026 :

- Les consultants indépendants utilisent en moyenne **4 à 6 outils différents** pour gérer leur activité client
- La gestion fragmentée des données est **la principale source d'inefficacité** pour les indépendants
- Les CRM existants sont soit **trop complexes** (Salesforce, HubSpot) soit **trop génériques** (Notion, Trello)
- Le besoin numéro 1 est la **centralisation** — contacts, missions, relances et facturation au même endroit
- Les consultants veulent un outil **opérationnel en moins de 24h**, pas une formation de 2 jours

### Concurrents directs
| Outil | Prix | Problème |
|---|---|---|
| HubSpot | Gratuit puis 45€/mois | Trop complexe pour un solo |
| Salesforce | 75€+/mois | Conçu pour les grandes équipes |
| Notion | 8€/mois | Pas conçu pour la vente |
| Less Annoying CRM | 15$/mois | Interface datée, pas adapté FR |
| Trello | Gratuit | Limité, pas de vision financière |

### Notre positionnement
**Simple, français, fait pour un seul utilisateur.** Pas de fonctionnalités inutiles. Pas de courbe d'apprentissage. Opérationnel en 10 minutes.

---

## 4. Fonctionnalités — MVP

### Must Have (v1.0)
- [ ] **Authentification** — Inscription / Connexion sécurisée
- [ ] **Gestion des clients** — Fiche client (nom, entreprise, email, téléphone, notes)
- [ ] **Pipeline de missions** — Statuts : Prospect → Devis envoyé → Mission en cours → Terminé
- [ ] **Relances** — Rappels manuels avec date et note
- [ ] **Dashboard** — Vue synthétique : clients actifs, missions en cours, relances du jour
- [ ] **Chiffre d'affaires** — Suivi simple du CA par client et par mois

### Should Have (v1.1)
- [ ] **Notes de mission** — Journal de bord par client
- [ ] **Tags et filtres** — Segmenter les clients par secteur ou type de mission
- [ ] **Export CSV** — Exporter ses données

### Nice to Have (v2.0)
- [ ] **Génération de devis** — Créer et envoyer un devis depuis l'app
- [ ] **Intégration calendrier** — Sync Google Calendar
- [ ] **Facturation simple** — Générer une facture PDF
- [ ] **Mode mobile** — PWA responsive

---

## 5. Stack technique

| Couche | Technologie | Raison |
|---|---|---|
| Frontend | React + Tailwind CSS | Moderne, composants réutilisables |
| Backend | Supabase | Auth + BDD PostgreSQL + API en un |
| Déploiement | Vercel | Gratuit, rapide, CI/CD automatique |
| Paiements | Stripe | Standard industrie |
| Tests | Vitest | Déjà maîtrisé |

---

## 6. Modèle économique

| Plan | Prix | Inclus |
|---|---|---|
| Gratuit | 0€ | 3 clients max, fonctions de base |
| Solo | 19€/mois | Clients illimités, toutes les fonctions |
| Pro | 39€/mois | Export, devis, facturation |

**Objectif 12 mois :** 100 clients Solo = 1 900€ MRR

---

## 7. Roadmap
Mai 2026      → PRD + maquettes Figma
Juin 2026     → Setup React + Supabase + Auth
Juillet 2026  → Gestion clients + Pipeline
Août 2026     → Dashboard + Relances
Sept 2026     → Beta privée (10 testeurs)
Oct 2026      → Lancement public + Stripe
---

## 8. Métriques de succès

- **Activation :** L'utilisateur ajoute son premier client en moins de 5 minutes
- **Rétention :** 60% des utilisateurs actifs après 30 jours
- **Conversion :** 10% des utilisateurs gratuits passent au plan payant
- **NPS :** Score supérieur à 40

---

## 9. Ce qu'on ne fera PAS (v1.0)

- Pas de gestion d'équipe multi-utilisateurs
- Pas d'intégration email automatique
- Pas d'IA générative
- Pas d'application mobile native

> *"Un bon produit fait peu de choses, mais les fait parfaitement."*

---

*Document vivant — mis à jour à chaque sprint.*