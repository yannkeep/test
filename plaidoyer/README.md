# #B!Mi — Plaidoyer Citoyen

<div align="center">

![Version](https://img.shields.io/badge/version-4.0-48bb78?style=for-the-badge)
![Licence](https://img.shields.io/badge/licence-CC%20BY--NC--SA%204.0-9f7aea?style=for-the-badge)
![Statut](https://img.shields.io/badge/statut-production-68d391?style=for-the-badge)

**Poste de travail numérique pour la participation citoyenne et l'éducation populaire**

[Lancer l'application](#-démarrage-rapide) • [Documentation](#-documentation) • [Contribuer](#-contribuer)

</div>

---

## 🎯 Qu'est-ce que c'est ?

**Plaidoyer Citoyen** est une application web gratuite et open source qui vous accompagne dans la construction d'une stratégie de plaidoyer structurée. Basée sur la méthodologie **Voir-Juger-Agir** issue de l'éducation populaire, elle propose 15 outils pour analyser votre situation, identifier vos leviers d'action et planifier votre campagne.

### ✨ Fonctionnalités principales

| Fonctionnalité | Description |
|----------------|-------------|
| 🔧 **15 outils méthodologiques** | Domino, SWOT, PESTEL, Arbre à problèmes, 5 Pourquoi, Théorie du changement... |
| 📊 **Tableau de bord** | Visualisation de votre progression par phase (Voir/Juger/Agir) |
| 👥 **Cartographie des acteurs** | Matrice pouvoir/intérêt interactive avec drag & drop |
| 📁 **Multi-projets** | Gérez plusieurs plaidoyers en parallèle |
| 💾 **Stockage local** | IndexedDB + localStorage fallback — vos données restent chez vous |
| 📤 **Export multiformats** | JSON, Markdown, HTML, CSV, PDF |
| 📥 **Import intelligent** | Compatible avec différents formats de données |
| 🎨 **Mode sombre** | Interface retro-geek vert tendre & lilas |
| 📱 **Responsive** | Fonctionne sur desktop, tablette et mobile |
| 🔒 **Hors-ligne** | Aucune connexion requise après le premier chargement |

---

## 🚀 Démarrage rapide

### Option 1 : Téléchargement direct

1. Téléchargez le fichier `plaidoyer-bimi-ultimate.html`
2. Ouvrez-le dans votre navigateur (Chrome, Firefox, Edge, Safari)
3. C'est prêt ! Vos données sont stockées localement.

### Option 2 : Depuis GitHub

```bash
git clone https://github.com/bimi-collective/plaidoyer-citoyen.git
cd plaidoyer-citoyen
# Ouvrez index.html dans votre navigateur
```

### Option 3 : En ligne

Accédez directement à : **https://bimi.tools/plaidoyer**

---

## 📚 Documentation

### La méthodologie Voir-Juger-Agir

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   🔵 VOIR          🟠 JUGER           🟢 AGIR              │
│   ─────────        ──────────         ─────────            │
│   Observer         Analyser           Planifier            │
│   Comprendre       Diagnostiquer      Mobiliser            │
│   Ressentir        Prioriser          Évaluer              │
│                                                             │
│   • Domino         • Acteurs          • Pouvoir            │
│   • Profil         • Arbre            • Cibles             │
│   • Fleur          • 5 Pourquoi       • SMART              │
│                    • SWOT             • Message            │
│                    • PESTEL           • Évaluation         │
│                    • TDC              • Journal            │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Les 15 outils

#### Phase VOIR (3 outils)

| Outil | Description |
|-------|-------------|
| **🎯 Domino du changement** | Clarifiez votre vision, identifiez les obstacles et ressources |
| **👤 Profil citoyen** | Analysez vos motivations, compétences, temps disponible et limites |
| **🌸 Fleur du pouvoir** | Explorez vos identités, privilèges et oppressions systémiques |

#### Phase JUGER (6 outils)

| Outil | Description |
|-------|-------------|
| **👥 Cartographie des acteurs** | Matrice pouvoir/intérêt pour identifier alliés et opposants |
| **🌳 Arbre à problèmes** | Visualisez causes (racines), problème (tronc) et conséquences (branches) |
| **❓ 5 Pourquoi** | Remontez à la cause racine par questionnement itératif |
| **📊 SWOT** | Forces, Faiblesses, Opportunités, Menaces |
| **🌍 PESTEL** | Analyse Politique, Économique, Social, Technologique, Environnemental, Légal |
| **🔄 Théorie du changement** | Modélisez le chemin de la situation actuelle vers la situation souhaitée |

#### Phase AGIR (6 outils)

| Outil | Description |
|-------|-------------|
| **⚡ Avec/Sans/Contre** | Trois postures stratégiques face au pouvoir |
| **🎯 Cibles & Alliés** | Identifiez vos cibles principales, secondaires et alliés stratégiques |
| **✅ Objectifs SMART** | Définissez des objectifs Spécifiques, Mesurables, Atteignables, Réalistes, Temporels |
| **💬 Message clé** | Structurez votre communication : accroche, problème, importance, cible, action |
| **📈 Suivi-évaluation** | Indicateurs, méthodes, calendrier et leçons apprises |
| **📔 Journal de bord** | Chronique de votre plaidoyer avec entrées datées |

---

## 💾 Gestion des données

### Stockage

Vos données sont stockées **localement** dans votre navigateur :
- **IndexedDB** (principal) : base de données performante
- **localStorage** (fallback) : si IndexedDB n'est pas disponible

⚠️ **Attention** : Vider le cache de votre navigateur supprimera vos données. Pensez à exporter régulièrement !

### Export

| Format | Extension | Usage |
|--------|-----------|-------|
| JSON | `.json` | Sauvegarde complète, ré-importable |
| Markdown | `.md` | Documentation, GitHub, wiki |
| HTML | `.html` | Rapport stylisé autonome |
| CSV | `.csv` | Tableur (Excel, LibreOffice) |
| PDF | `.pdf` | Impression, partage formel |

### Import

L'application accepte plusieurs formats :
- **Format natif** : exports JSON de l'application
- **Format dataset** : structure compatible avec les templates

---

## 🎨 Personnalisation

### Thème

L'interface utilise un design "retro-geek" en mode sombre avec :
- **Vert tendre (mint)** : couleur principale `#48bb78`
- **Lilas** : couleur secondaire `#9f7aea`
- **Fond sombre** : nuances de `#0d0d14` à `#222233`

### Templates disponibles

| Template | Description |
|----------|-------------|
| **Projet vierge** | Structure vide pour démarrer de zéro |
| **Stop Arizona** | Exemple de plaidoyer contre les réformes sociales belges |
| **ECP** | Économie Contributive Provisionnée — plaidoyer pour l'innovation sociale |

---

## 🛠️ Architecture technique

```
plaidoyer-bimi-ultimate.html
├── HTML5 sémantique
├── CSS3 (variables, grid, flexbox)
├── JavaScript vanilla (ES6+)
├── IndexedDB (stockage)
└── Web APIs (FileReader, Blob, URL)
```

**Aucune dépendance externe** hormis les polices Google Fonts (Space Grotesk, JetBrains Mono).

### Compatibilité navigateurs

| Navigateur | Version minimum |
|------------|-----------------|
| Chrome | 80+ |
| Firefox | 75+ |
| Safari | 13+ |
| Edge | 80+ |

---

## 🤝 Contribuer

Les contributions sont les bienvenues ! 

### Comment contribuer

1. **Fork** le repository
2. Créez une **branche** (`git checkout -b feature/ma-fonctionnalite`)
3. **Committez** vos changements (`git commit -am 'Ajout de ma fonctionnalité'`)
4. **Push** vers la branche (`git push origin feature/ma-fonctionnalite`)
5. Ouvrez une **Pull Request**

### Types de contributions

- 🐛 Signaler des bugs
- 💡 Proposer des fonctionnalités
- 📝 Améliorer la documentation
- 🌍 Traduire l'interface
- 🎨 Améliorer le design
- 🧪 Ajouter des tests

---

## 📄 Licence

Ce projet est sous licence **Creative Commons BY-NC-SA 4.0**.

Vous êtes libre de :
- **Partager** — copier et redistribuer le matériel
- **Adapter** — remixer, transformer et créer à partir du matériel

Selon les conditions suivantes :
- **Attribution** — Vous devez créditer #B!Mi Collective
- **Pas d'utilisation commerciale** — Pas d'usage commercial sans autorisation
- **Partage dans les mêmes conditions** — Même licence pour les dérivés

---

## 🙏 Crédits

### Méthodologie
- **Voir-Juger-Agir** : Mouvement de la Jeunesse Ouvrière Chrétienne (JOC), 1925
- **Éducation populaire** : Paulo Freire, *Pédagogie des opprimés*, 1968
- **Fleur du pouvoir** : Adapté de l'outil de conscientisation féministe

### Ressources
- [Guide du plaidoyer citoyen](https://www.cncd.be) — CNCD-11.11.11
- [Manuel de l'éducation permanente](https://www.cesep.be) — CESEP
- [Outils d'analyse stratégique](https://www.youropa.be) — YourOpa

### Technologies
- Polices : [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono)
- Icônes : Emoji natifs Unicode

---

## 📞 Contact

- **Email** : contact@bimi.tools
- **GitHub** : [github.com/bimi-collective](https://github.com/bimi-collective)
- **Mastodon** : [@bimi@social.coop](https://social.coop/@bimi)

---

<div align="center">

**Fait avec ❤️ par le collectif #B!Mi**

*Pour une démocratie participative et une citoyenneté active*

</div>
