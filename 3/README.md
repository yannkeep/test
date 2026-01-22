Je vais analyser les deux versions pour créer la fusion ultime. Laissez-moi d'abord examiner les deux approches.Maintenant je comprends les deux approches ! Laissez-moi créer la fusion ultime.Je vais créer la version ultime fusionnée. C'est un gros fichier, je vais le construire méthodiquement.## #B!Mi — Plaidoyer Citoyen ULTIMATE v4.0

Voici la fusion des deux versions avec toutes les spécifications documentées :

---

### 🎨 DESIGN SYSTEM — Rétro Geek Vert Tendre & Lilas

| Élément | Valeur | Usage |
|---------|--------|-------|
| **Fond principal** | `#12121a` | Background base |
| **Fond élevé** | `#1a1a26` | Cards, panels |
| **Surface** | `#222233` | Inputs, hover |
| **Bordure** | `#2d2d44` → `#4d4d66` | Subtile → Strong |
| **Vert tendre (Mint)** | `#48bb78` → `#68d391` | Accent principal |
| **Lilas** | `#805ad5` → `#9f7aea` | Accent secondaire |
| **Glow mint** | `rgba(72, 187, 120, 0.3)` | Ombres lumineuses |
| **Glow lilas** | `rgba(159, 122, 234, 0.3)` | Accents visuels |

**Phases** :
- VOIR : `#63b3ed` (bleu ciel)
- JUGER : `#f6ad55` (orange)
- AGIR : `#68d391` (vert)

---

### 🔤 TYPOGRAPHIE

| Type | Police | Usage |
|------|--------|-------|
| Display | `Space Grotesk` | Titres, UI |
| Mono | `JetBrains Mono` | Données, badges, code |

---

### 📐 LAYOUT & RESPONSIVE

| Breakpoint | Comportement |
|------------|--------------|
| `>1024px` | Sidebar fixe (280px) + Main |
| `<1024px` | Header fixe + Sidebar drawer |

**Dimensions** :
- Header : 56px
- Sidebar : 280px
- Max content : 900px

---

### 💾 STOCKAGE

| Méthode | Description |
|---------|-------------|
| **IndexedDB** | `BimiPlaidoyerDB` → Store `projects` |
| **Fallback** | `localStorage` clé `bimi_projects` |
| **Auto-save** | Debounce 800ms |

---

### 📋 MODÈLE DE DONNÉES

```javascript
{
  id: "timestamp",
  meta: { name, description, created, updated },
  domino: { vision, obstacles, ressources },
  profil: { motivations, competences, temps, limites },
  fleur: { identites, privileges, oppressions },
  acteurs: [{ id, name, role, position, power }],
  arbre: { probleme, causes, consequences },
  pourquoi: { p1, p2, p3, p4, p5 },
  swot: { forces, faiblesses, opportunites, menaces },
  pestel: { p, e, s, t, en, l },
  tdc: { actuelle, souhaitee, mecanismes, hypotheses },
  pouvoir: { avec, sans, contre },
  cibles: { principales, secondaires, allies },
  message: { accroche, probleme, importance, cible, action },
  evaluation: { indicateurs, methodes, calendrier, lecons },
  smart: [{ id, text, indicator, deadline, done }],
  journal: [{ id, date, content }]
}
```

---

### 🛠️ 15 OUTILS MÉTHODOLOGIQUES

**VOIR (3)** : Domino • Profil • Fleur du pouvoir

**JUGER (6)** : Cartographie acteurs • Arbre à problèmes • 5 Pourquoi • SWOT • PESTEL • Théorie du changement

**AGIR (6)** : Avec/Sans/Contre • Cibles & Alliés • Objectifs SMART • Message clé • Suivi-évaluation • Journal de bord

---

### 📥📤 IMPORT / EXPORT

| Format | Extension | Support |
|--------|-----------|---------|
| JSON | `.json` | Natif + formats legacy |
| Markdown | `.md` | Export structuré |
| HTML | `.html` | Document standalone |
| CSV | `.csv` | Tableur |

---

### 🎓 DIDACTICIEL NON-INVASIF

- **Help tooltips** : Icône `?` au survol → clic pour afficher
- **Position** : Près de l'élément cliqué
- **Fermeture** : Clic ailleurs ou `Esc`
- **Contenu** : Concis, factuel, adulte (pas de "!" excessifs)
- **Dictionnaire HELP** : 15 entrées contextuelles

---

### ⌨️ RACCOURCIS CLAVIER

| Raccourci | Action |
|-----------|--------|
| `Ctrl+K` | Recherche globale |
| `Ctrl+S` | Sauvegarder |
| `Esc` | Fermer modal/tooltip |

---

### 📊 CALCUL PROGRESSION

```javascript
VOIR = (champs_remplis_domino + profil + fleur) / 10
JUGER = (champs_arbre + pourquoi + swot + pestel + tdc + acteurs) / 20
AGIR = (champs_pouvoir + cibles + message + evaluation + smart + journal) / 15
GLOBAL = moyenne(VOIR, JUGER, AGIR)
```

---

### 🎭 TEMPLATES PRÉ-REMPLIS

1. **Projet vierge** : Structure vide
2. **Stop Arizona** : Données démo complètes (acteurs, objectifs SMART)

---

### 🌐 SEO / SCHEMA.ORG

- Meta tags complets (Open Graph, description)
- JSON-LD `WebApplication`
- Canonical URL
- PWA-ready (`theme-color`, `apple-mobile-web-app`)

---

**Logo** : `#B!Mi` affiché dans un carré dégradé mint→lilas avec glow
