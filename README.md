# Camping Ti Piton — choix du site

Site de présentation **KréaPro** pour le Camping Ti Piton (Îlet des Orangers, Mafate) : le client parcourt tous les
modèles, met un ♡ sur ceux qui lui plaisent, choisit son préféré et envoie son choix avec ses commentaires.

- `index.html` — page « Choisissez votre site », 44 modèles en 3 groupes :
  1. **Les 8 propositions du devis** (formule Salazie, 790 €) : Le manifeste, Lettres-fenêtres, Grand angle,
     Carte postale, chacun avec ses vraies photos ou avec des images générées d'après ses photos ;
  2. **Plus de styles, avec ses vraies photos** (9) : Salazie, ou Mafate (2 690 €) pour les modèles à effets ;
  3. **Plus de styles, avec des images d'ambiance** générées par IA, qui ne montrent pas le camping (27).
  - Chaque carte indique le type d'images et la formule.
  - Formulaire « Mon choix » : le préféré, les ♡ et les commentaires partent par **WhatsApp** (0693 86 08 02) ou par
    **e-mail** (contact@kreapro.re), sans serveur.
- `modeles/` — les 44 maquettes. En haut, une barre « ← Tous · ♡ J'aime · ★ Je choisis ». Les autres liens (appeler,
  WhatsApp, e-mail…) sont neutralisés pour que le client reste dans le parcours.
- `images/` — uniquement les images utilisées, plus les aperçus des cartes (`images/apercus/<n°>.webp`).
- `vercel.json` + `robots.txt` + balises `noindex` : le site n'est pas indexé par les moteurs de recherche.

## Mise en ligne sur Vercel
Site statique, sans étape de construction : *Add New… → Project → importer ce dépôt*, préréglage **Other**, dossier
racine `./`, pas de commande de build. Choisir la branche à publier dans *Settings → Git → Production Branch*.

## Mise à jour
Le contenu est généré par `site-demo/_generation/vercel_build.py` (dossier de travail KréaPro), puis commité ici.

Maquettes réalisées par KréaPro — les sites ne sont pas encore en ligne.
