# Mission #0 ULTRA — Éditeur Markdown

## 📁 Structure des fichiers

```
ton-dossier/
├── index.html          ← renomme Mission_0_ULTRA.html en index.html
└── markdown/           ← crée ce dossier
    ├── guide.md
    ├── offre.md
    ├── mission.md
    ├── WARNING.md
    └── ... (tes fichiers .md)
```

---

## ⚙️ Configuration du préchargement

Ouvre le fichier HTML et cherche ce bloc (vers la ligne 130 du script) :

```javascript
// ========== LISTE DES FICHIERS À PRÉCHARGER ==========
// Ajoute tes fichiers .md ici, ils seront chargés depuis ./markdown/
const markdownFiles = [
  'guide.md',
  'offre.md',
  'WARNING.md',
  'avertissement.md',
  'mission.md',
  'service.md',
  'man.md',
  'sauron.md',
  'postuler.md',
  'partenariat.md',
  'omg.md',
  'dossier_blanc.md',
  '5_verites.md',
  'plan-b.md'
];
```

**Modifie ce tableau** avec les noms exacts de tes fichiers dans le dossier `./markdown/`

---

## 🚀 Utilisation

1. Place tes fichiers `.md` dans le dossier `markdown/`
2. Liste leurs noms dans le tableau `markdownFiles`
3. Ouvre `index.html` dans un navigateur (via un serveur local)

### ⚠️ Important : Serveur local requis

Le chargement des fichiers `.md` utilise `fetch()`, donc tu dois utiliser un serveur local :

**Option 1 — Python :**
```bash
cd ton-dossier
python -m http.server 8000
# puis ouvre http://localhost:8000
```

**Option 2 — Node.js :**
```bash
npx serve ton-dossier
```

**Option 3 — VS Code :**
Installe l'extension "Live Server" et clique sur "Go Live"

**Option 4 — PHP :**
```bash
cd ton-dossier
php -S localhost:8000
```

---

## ⌨️ Raccourcis clavier

| Raccourci | Action |
|-----------|--------|
| `Ctrl+S` | Sauvegarder (télécharge le fichier) |
| `Ctrl+N` | Nouveau fichier |
| `Ctrl+E` | Export MD |
| `Ctrl+R` | Rafraîchir les fichiers |
| `Ctrl+B` | **Gras** |
| `Ctrl+I` | *Italique* |
| `Ctrl+K` | Lien |
| `Ctrl+1` | Vue Split |
| `Ctrl+2` | Vue Éditeur seul |
| `Ctrl+3` | Vue Preview seul |

---

## ✨ Fonctionnalités

- **Prévisualisation live** du Markdown
- **Coloration syntaxique** du code (highlight.js)
- **Diagrammes Mermaid** supportés
- **Drag & drop** de fichiers .md
- **Export MD et HTML**
- **Mode sombre** avec effets visuels (particules, aurora, glassmorphism)
- **Responsive** (adapté mobile)

---

## 📝 Exemple de fichier Markdown

```markdown
# Mon Titre

Ceci est un paragraphe avec du **gras** et de l'*italique*.

## Code

\`\`\`javascript
const hello = "Hello World";
console.log(hello);
\`\`\`

## Liste

- Item 1
- Item 2
- Item 3

## Citation

> Une citation importante

## Diagramme Mermaid

\`\`\`mermaid
graph LR
    A[Début] --> B[Milieu]
    B --> C[Fin]
\`\`\`

## Tableau

| Colonne 1 | Colonne 2 |
|-----------|-----------|
| Valeur A  | Valeur B  |
| Valeur C  | Valeur D  |
```

---

## 🎨 Personnalisation des couleurs

Les couleurs sont définies dans les variables CSS au début du fichier :

```css
:root{
  --bg:#030308;              /* Fond principal */
  --panel:rgba(12,14,28,0.7); /* Panneaux */
  --text:#e8eaf0;            /* Texte */
  --lilac:#b19cd9;           /* Accent lilas */
  --green:#00ff88;           /* Accent vert */
  --cyan:#00f0ff;            /* Accent cyan */
  /* ... */
}
```

---

## 📂 Ajouter/Retirer des fichiers

Pour ajouter un nouveau fichier :

1. Place `mon-nouveau-fichier.md` dans `./markdown/`
2. Ajoute `'mon-nouveau-fichier.md'` dans le tableau `markdownFiles`
3. Rafraîchis la page (ou clique sur 🔄 Refresh)

Pour retirer un fichier :

1. Supprime le nom du tableau `markdownFiles`
2. (Optionnel) Supprime le fichier du dossier `./markdown/`

---

## 🐛 Problèmes courants

### Les fichiers ne se chargent pas
→ Tu dois utiliser un serveur local (voir section ci-dessus)

### Fichier non trouvé
→ Vérifie que le nom dans `markdownFiles` correspond exactement au nom du fichier (sensible à la casse)

### Mermaid ne s'affiche pas
→ Utilise la syntaxe :
```
\`\`\`mermaid
graph LR
    A --> B
\`\`\`
```

---

## 📜 Licence

Libre d'utilisation et de modification.

---

*Mission #0 ULTRA — Version sublimée avec particules, aurora, glassmorphism et mode sombre.*
