# 🎵 SonicCore — Système de supervision audio multi-sites

> Plateforme de supervision et de diffusion musicale continue pour environnements multi-sites (entreprises, collectivités, campus, gares...), avec gestion des alertes, synchronisation des playlists et tableau de bord en temps réel.

⚠️ **Projet en cours de développement** - Date de rendu : juin 2026

---

## 📌 Contexte

Projet fil rouge réalisé dans le cadre de la formation **BUT Informatique** (IUT de Villetaneuse, Université Sorbonne Paris Nord).

Dans de nombreuses organisations, assurer une **diffusion musicale continue** est un enjeu opérationnel réel : insertion de publicités programmées, messages d'urgence prioritaires, continuité de service même en cas de coupure réseau. Ce projet répond à ce besoin en mettant en place un système de supervision centralisé.

---

## 👥 Équipe

| Nom | Formation |
|---|---|
| Nassim BERRABAH | BUT Informatique — Sciences des Données |
| Nassim DADDA | BUT Informatique — Sciences des Données |
| Khardiata DIOP | BUT Informatique — Sciences des Données |

---

## 🎯 Fonctionnalités cibles

### Supervision
- Suivi en temps réel de l'état des lecteurs audio (**UP / KO**)
- Tableau de bord : état, synchronisation, "now playing"
- Déclenchement d'**alertes automatiques** (lecteur KO, playlist obsolète, absence de diffusion)

### Gestion des playlists
- Mise à jour centralisée des playlists locales
- Synchronisation automatique sur les lecteurs distants
- Vérification de la playlist de secours (continuité en cas de coupure réseau)

### Historique & logs
- Consignation de tous les messages diffusés (musique, publicité, urgent)
- Stockage de l'historique des événements et incidents

### Scénarios de test prévus
- Coupure réseau
- Coupure électrique
- Diffusion d'un message urgent
- Respect du planning des publicités

---

## 🏗️ Architecture du projet

```
SonicCore
├── Site vitrine WordPress     ← Présentation du projet / produit
├── Back-end Laravel           ← API REST, gestion des lecteurs, alertes, logs
└── Front-end Vue.js           ← Tableau de bord de supervision en temps réel
```

**Pilote prévu :**
- 1 site principal
- 2 sites distants
- 2 lecteurs de test

---

## 🛠️ Stack technique

| Couche | Technologie |
|---|---|
| Front-end | Vue.js |
| Back-end | Laravel (PHP) |
| Base de données | MySQL |
| Site vitrine | WordPress + Elementor |
| Versioning | Git / GitHub |

---

## 📅 Avancement

- [x] Définition du cahier des charges
- [x] Choix de la stack technique
- [ ] Site vitrine WordPress
- [ ] Modélisation de la base de données
- [ ] API Laravel (lecteurs, playlists, alertes)
- [ ] Tableau de bord Vue.js
- [ ] Synchronisation des playlists
- [ ] Scénarios de test

---

## 📁 Structure du repo

```
📦 soniccore
 ┣ 📂 back/          ← API Laravel
 ┣ 📂 front/         ← Application Vue.js
 ┣ 📂 wordpress/     ← Export / thème du site vitrine
 ┣ 📄 README.md
 ┗ 📄 .gitignore
```

---

## 👤 Contact

**Nassim Berrabah** - BUT Informatique, Sciences des Données  
IUT de Villetaneuse, Université Sorbonne Paris Nord  
