# Camping Ti Piton — choix du site

Site de présentation **KréaPro** pour le Camping Ti Piton (Îlet des Orangers, Mafate) : le client choisit le modèle de son
futur site (formule Salazie) et envoie son choix et ses commentaires.

- `index.html` — page « Choisissez votre site » : 4 styles × 2 types d'images
  - **Avec vos vraies photos** : Le manifeste, Lettres-fenêtres, Grand angle, Carte postale ;
  - **Avec des images générées d'après vos photos** (illustrations IA) : les 4 mêmes styles ;
  - formulaire « Mon choix » : le choix et les commentaires partent par **WhatsApp** (0693 86 08 02) ou par **e-mail**
    (contact@kreapro.re), sans serveur.
- `modeles/` — les 8 maquettes. Une barre « ← Tous les modèles · ★ Je choisis celui-ci » en haut ; les autres liens
  (appeler, WhatsApp, e-mail…) sont neutralisés pour que le client reste dans le parcours.
- `images/` — uniquement les images utilisées.
- `vercel.json` + `robots.txt` + balises `noindex` : le site n'est pas indexé par les moteurs de recherche.

## Mise en ligne sur Vercel
Site statique, sans étape de construction : *Add New… → Project → importer ce dépôt*, préréglage **Other**, dossier
racine `./`, pas de commande de build. Choisir la branche à publier dans *Settings → Git → Production Branch*.

## Mise à jour
Le contenu est généré par `site-demo/_generation/vercel_build.py` (dossier de travail KréaPro), puis commité ici.

Maquettes réalisées par KréaPro — les sites ne sont pas encore en ligne.
