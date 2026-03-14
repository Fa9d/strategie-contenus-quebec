# Conventions — Gestion des images

---

## Structure des dossiers

```
assets/
├── branding/                  ← Fichiers source (Canva, Figma, SVG) du branding global
└── images/
    ├── branding/              ← Logo, icônes, éléments visuels de l'identité du projet
    │   └── mesange.png        ← Logo principal du projet
    ├── sante/                 ← Visuels pour les contenus santé
    ├── crimes_canada/         ← Visuels pour les contenus Crimes du Canada
    ├── independance/          ← Visuels pour les contenus souveraineté / indépendance
    ├── energie/               ← Visuels pour les contenus énergie (Hydro-Québec, etc.)
    ├── services_publics/      ← Visuels pour les contenus services publics
    └── divers/                ← Captures d'écran, images non classées
```

> **Pour ajouter un nouveau thème :** créer simplement un nouveau sous-dossier dans `images/` avec le nom du thème en minuscules et sans espaces (ex. `images/logement/`).

---

## Convention de nommage des fichiers

### Format général

```
AAAA-MM-DD_slug-du-sujet_description-courte.ext
```

### Exemples

| Fichier | Usage |
|---|---|
| `mesange.png` | Logo principal (exception : pas de date sur les assets branding) |
| `2026-03-13_hydro-quebec_alerte-decembre.png` | Capture d'écran d'une alerte HQ |
| `2026-03-13_hydro-quebec_graphique-exportations.jpg` | Graphique extrait d'un rapport |
| `2026-03-15_sante_temps-attente-urgences-2025.png` | Statistique visuelle santé |

### Règles
- **Minuscules uniquement**, pas d'accents, pas d'espaces → utiliser `-` comme séparateur.
- **Toujours dater** les images récupérées sur le net (date de récupération si la date originale est inconnue).
- **Extension en minuscule** : `.png`, `.jpg`, `.svg`, `.webp` — jamais `.PNG` ou `.JPG`.
- **Préférer `.png`** pour les captures d'écran et graphiques (sans perte), **`.jpg`** pour les photos.
- **SVG** pour les icônes et illustrations vectorielles.

---

## Images récupérées sur le web

### À toujours noter (dans la fiche de recherche associée)

| Champ | Exemple |
|---|---|
| Fichier local | `assets/images/energie/2026-03-13_hydro-quebec_graphique-exportations.jpg` |
| Source originale | `https://www.hydroquebec.com/...` |
| Auteur / organisation | Hydro-Québec |
| Date de publication originale | 2025-11-15 |
| Licence / droits | © Hydro-Québec — usage éditorial non commercial |
| Date de téléchargement | 2026-03-13 |

### Règles légales et éditoriales
- **Ne jamais publier** une image sous copyright sans transformation (montage, citation, critique) ou permission explicite.
- **Préférer** les sources libres de droits : Unsplash, Wikimedia Commons, publications gouvernementales en accès libre.
- **Pour les captures d'écran** de documents officiels, de manchettes ou de tweets : usage éditorial généralement couvert par la doctrine de la citation — documenter la source.
- **Toujours créditer** dans les contenus publiés quand la licence l'exige.

---

## Ce que Git track / n'track pas

| Type | Tracké ? | Raison |
|---|---|---|
| `.png`, `.jpg`, `.svg`, `.webp` (< 5 Mo) | ✅ Oui | Assets utiles, taille raisonnable |
| `.psd`, `.ai`, `.eps` | ❌ Non | Fichiers source lourds Photoshop/Illustrator |
| `.raw`, `.cr2`, `.nef`, `.arw` | ❌ Non | Photos brutes, très lourdes |
| `.mp4`, `.mov`, `.avi` | ❌ Non | Vidéos (voir règle dans `.gitignore`) |

> **Images très lourdes (> 5 Mo) :** les stocker dans un dossier `exports/` local (ignoré par Git) ou utiliser Git LFS si nécessaire.
