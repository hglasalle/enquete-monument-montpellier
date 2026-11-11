# Enquête interactive — Le monument aux morts de Montpellier

Application web (une seule page, sans dépendance) qui transforme la fiche élève
**« Le monument aux morts de Montpellier — matériaux, gestes et symboles »** en
une enquête interactive de style Genially, pensée pour l’iPad.

## Contenu

- 4 chapitres, 12 questions, un croquis légendé et une question bonus.
- Textes, questions et indices **repris à l’identique** de la fiche élève.
- Choix multiples, réponses libres, carte des fronts, croquis au doigt/stylet.
- Indices, points, tampons collectés, carnet d’enquête final.
- Sauvegarde automatique des réponses sur l’appareil (localStorage).
- Impression / export PDF et téléchargement du carnet en `.txt`.
- Interface tactile : grandes cibles, balayage gauche/droite, plein écran iOS.
- Habillage « papier ancien » évoquant la Première Guerre mondiale et les tranchées,
  avec une photographie du monument aux morts de Montpellier.

## Utilisation en classe

1. Ouvrir l’URL GitHub Pages sur l’iPad (Safari).
2. Éventuellement : **Partager → Sur l’écran d’accueil** pour un affichage plein écran.
3. Chaque élève ou groupe répond sur son appareil ; le carnet final peut être
   imprimé, exporté en PDF (AirPrint) ou téléchargé.

> Les réponses sont enregistrées dans le navigateur de l’appareil. Le bouton
> « Recommencer » efface les réponses après confirmation.

## Structure

```
index.html   → toute l’application (HTML + CSS + JS, illustrations SVG intégrées)
assets/      → photographie du monument aux morts (facultative)
README.md    → ce fichier
.nojekyll    → empêche GitHub Pages d’ignorer certains fichiers
```

## Publication

Le site est statique : aucun build, aucune dépendance.

### GitHub Pages

1. Créer un dépôt public.
2. Déposer `index.html`, `README.md` et `.nojekyll` à la racine.
3. **Settings → Pages → Deploy from a branch → main / (root)**.
4. L’adresse est de la forme `https://<compte>.github.io/<depot>/`.

> Si `assets/monument-montpellier.jpg` est absent, le site charge automatiquement
> la photographie depuis Wikimedia Commons (nécessite une connexion Internet).

### En local

Ouvrir `index.html` dans un navigateur suffit. Pour que la sauvegarde
fonctionne de façon fiable, servir le dossier avec un petit serveur HTTP
(`python -m http.server`, par exemple).

## Source

Fiche élève : *Fiche_eleve_monument_aux_morts_Montpellier_mise_en_page.pdf*.
Les intitulés des chapitres et les libellés d’interface ont été ajoutés pour
la mise en scène ; les questions, consignes et indices du document n’ont pas
été modifiés.

## Crédit photographique

*War memorial Montpellier* — Andrew Dalby, **domaine public** (PD-self),
via Wikimedia Commons :
<https://commons.wikimedia.org/wiki/File:War_memorial_Montpellier.JPG>.
La photographie est recadrée et légèrement sépia pour l’habillage du site.
