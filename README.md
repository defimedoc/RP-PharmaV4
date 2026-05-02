# romainpoulin.fr — CV Personnel

Site CV statique de Romain Poulin, Docteur en Pharmacie et Directeur Opérationnel chez [Défimédoc](https://www.defimedoc.fr).

Déployé via **GitHub Pages** sur [romainpoulin.fr](https://romainpoulin.fr).

---

## Stack

- HTML5 / CSS3 / JavaScript vanilla
- Zéro dépendance, zéro framework
- Google Fonts (Lato) — seule ressource externe

## Structure

```
/
├── index.html      # Site complet (single-page)
├── pp.jpg          # Photo de profil
├── CNAME           # Domaine custom GitHub Pages
└── README.md
```

## Fonctionnalités

- Single-page app avec navigation par sections (Accueil, À propos, CV)
- Mode **light / dark** avec mémorisation (`localStorage`)
- **Responsive mobile** avec menu burger et drawer plein écran
- CV en onglets (Parcours / Formations & Compétences)
- Timeline visuelle avec dot animé pour le poste actuel
- Tags de compétences hiérarchisés (Maîtrisé / Notions / Langues)
- SEO optimisé : meta, Open Graph, Schema.org `Person` (JSON-LD)

## Déploiement

Le site est déployé automatiquement par GitHub Pages à chaque push sur la branche `main`.

### DNS à configurer chez ton registrar

| Type  | Nom | Valeur |
|-------|-----|--------|
| A     | @   | 185.199.108.153 |
| A     | @   | 185.199.109.153 |
| A     | @   | 185.199.110.153 |
| A     | @   | 185.199.111.153 |
| CNAME | www | Trydrica.github.io |

> Les enregistrements A pointent vers les serveurs GitHub Pages.  
> Le CNAME `www` redirige vers `romainpoulin.fr`.

## Mise à jour du contenu

Tout le contenu est dans `index.html`. Rechercher les balises de section :

- `<!-- HOME -->` — photo, nom, titre, boutons
- `<!-- À PROPOS -->` — texte de présentation
- `<!-- CV -->` — timeline parcours, formations, compétences

## Licence

© 2023–2025 Romain Poulin — Tous droits réservés.
