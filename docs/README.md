# Stratégie Contenus Québec

## Vision du projet

Ce dépôt centralise la production de contenus politiques sur le Québec : santé publique, souveraineté, critique du fédéralisme canadien, défense des services publics. L'objectif est de produire des contenus rigoureux, accessibles et percutants — ancrés dans les faits, orientés vers l'action citoyenne.

---

## Thèmes principaux

| Thème | Description |
|---|---|
| Santé | Sous-financement, liste d'attente, comparaisons provinciales et internationales |
| Crimes du Canada | Pensionnats, spoliations, politiques d'assimilation, mémoire historique |
| Indépendance | Arguments économiques, culturels et démocratiques pour la souveraineté |
| Services publics | Défense de l'éducation, transport, aide sociale contre le désengagement fédéral |

---

## Rôle des réseaux

### TikTok / Reels (Instagram)
- **Format :** 60–90 secondes, portrait
- **Rôle :** Séduire un public jeune (18–35 ans), créer un choc cognitif rapide, donner envie d'en savoir plus.
- **Ton :** Direct, énergique, visuel, pas condescendant.
- **KPI :** Vues, partages, sauvegardes.

### Instagram (carrousels)
- **Format :** 6–8 slides statiques ou animées
- **Rôle :** Expliquer en profondeur un fait ou un enjeu de façon lisible sur mobile.
- **Ton :** Épuré, chiffres mis en valeur, call-to-action fort en dernière slide.
- **KPI :** Sauvegardes, partages en story, abonnements.

### YouTube
- **Format :** 8–20 minutes, paysage
- **Rôle :** Ancrage éditorial. C'est ici que la recherche est déployée dans toute sa profondeur. Référence pour les médias, journalistes, militants.
- **Ton :** Structuré, analytique, pédagogique, engagé mais sourcé.
- **KPI :** Rétention, abonnements, partages longs.

### X / LinkedIn
- **Format :** Thread 5–8 tweets ou article long
- **Rôle :** Atteindre les décideurs, journalistes, analystes, militants organisés. Générer du débat public.
- **Ton :** Incisif sur X, plus posé sur LinkedIn.
- **KPI :** Impressions, retweets, engagements qualitatifs.

---

## Workflow global

```
IDÉE / ACTUALITÉ
      ↓
Fiche de recherche (research/_template_fiche_sujet.md)
      ↓
Validation éditoriale (cohérence, angle, lignes éditoriales)
      ↓
Script(s) selon les formats retenus
      ↓
Production (tournage / design / montage)
      ↓
Publication planifiée (planning/contenus.csv)
      ↓
Bilan engagement + archivage
```

---

## Structure du dépôt

```
strategie-contenus-quebec/
├── docs/
│   ├── README.md                    ← Ce fichier
│   └── lignes_editoriales.md        ← Charte éditoriale
├── research/
│   ├── _template_fiche_sujet.md     ← Template de fiche
│   ├── sante/
│   ├── crimes_canada/
│   └── independance/
├── scripts/
│   ├── tiktok_reels/
│   │   └── _template_tiktok.md
│   ├── youtube/
│   │   └── _template_youtube.md
│   ├── instagram/
│   │   └── _template_carrousel.md
│   └── x_linkedin/
│       └── _template_thread.md
├── assets/
│   ├── images/
│   └── branding/
└── planning/
    └── contenus.csv
```
