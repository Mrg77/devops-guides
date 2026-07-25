# DevOps — guides de projets

Des fiches web pour comprendre chacun de mes projets DevOps : ce que fait chaque
fonctionnalité, quand s'en servir et pourquoi. Toutes partagent la même identité
visuelle.

**En ligne :** https://mrg77.github.io/devops-guides/

## Contenu

| Fichier | Rôle |
|---|---|
| `index.html` | Page d'accueil — le sommaire des guides. |
| `opsforge-guide.html` | Guide du projet [opsforge](https://github.com/Mrg77/opsforge). |
| `devops-guide.css` | **La DA partagée** — couleurs, typo, composants. Réutilisée par chaque page. |
| `_TEMPLATE.html` | Gabarit vierge pour créer la page d'un nouveau projet. |

## Ajouter un nouveau projet

```sh
cp _TEMPLATE.html mon-projet-guide.html
# remplir les {{placeholders}}, dupliquer les blocs section/card
# puis ajouter une carte dans index.html
```

Le design vit dans `devops-guide.css` — réutilisé tel quel ; on surcharge juste
la couleur d'accent (`--accent`) par page si besoin. Thème clair/sombre
automatique, responsive.

## Publication

Servi par **GitHub Pages** depuis la branche `main` (racine). Un `.nojekyll`
désactive le traitement Jekyll pour que tous les fichiers soient servis tels
quels.
