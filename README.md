# Craftoura — coaching couture

Site vitrine statique (HTML / CSS / JS, sans build) hébergé sur GitHub Pages,
domaine `craftoura.shop`.

> Généré depuis `C:\Users\souha\coaching-sites-factory` (fichier `sites/craftoura.mjs`).
> Pour une modification de contenu, éditez ce fichier puis relancez `node build.mjs craftoura` :
> une modification faite directement ici serait écrasée à la prochaine génération.

## À compléter avant de communiquer sur le site

| Priorité | Quoi | Où |
|---|---|---|
| 🔴 Bloquant | Mentions légales : identité de l’éditeur, SIREN, adresse, médiateur. Obligatoire en France. | `mentions-legales.html` |
| 🟠 Important | Adresse `contact@craftoura.shop` : créer une redirection e-mail chez Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Formulaire : remplacer `VOTRE_ID_FORMSPREE` (sinon repli automatique en `mailto:`). | `contact.html` |
| 🟠 Important | Présentation de la personne qui coache (nom, parcours réel, photo). | `a-propos.html` |
| 🟡 Plus tard | Tarifs (25 / 59 / 129 €) et contenu des formules à ajuster à votre offre réelle. | `index.html` `#tarifs` |
| 🟡 Plus tard | Témoignages : n’en ajoutez que des vrais, avec l’accord des personnes. | — |

## Description de l’activité (Stripe, annuaires…)

```
Coaching en couture, 100 % en ligne : ateliers en direct en petit groupe et cours individuels en visioconférence portant sur la prise en main de la machine, la lecture et l’ajustement des patrons, les retouches et réparations de vêtements, et la réalisation d’une garde-robe cousue soi-même. Les élèves suivent un programme de 8 à 12 semaines avec des retours en photo sur leurs réalisations. Aucun tissu, patron papier ni matériel n’est vendu ni expédié. Les prestations sont vendues sous forme d’abonnements mensuels sans engagement, de 25 € à 129 € par mois, résiliables à tout moment. Site : craftoura.shop
```

## Structure

```
index.html            Accueil : hero, programmes, méthode, tarifs, approche, FAQ
programmes.html       Détail des 4 programmes
a-propos.html         Notre approche et principes
contact.html          Formulaire de prise de contact
mentions-legales.html Mentions légales, confidentialité, CGV
404.html              Page d’erreur (chemins absolus)
assets/css/style.css  Couleurs de la marque en tête de fichier, puis styles communs
assets/js/main.js     Menu, thème, animations, formulaire
```

## DNS (Namecheap → Advanced DNS)

Supprimer les enregistrements de parking, puis :

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
