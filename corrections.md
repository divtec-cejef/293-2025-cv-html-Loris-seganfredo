## A) Ajouter Normalize.css en local + corriger les liens CSS
- `normalize.css` doit être en local dans `./css/normalize.css`
- Veuillez garder uniquement ces deux liens (dans cet ordre) :
```
<link rel="stylesheet" href="./css/normalize.css">
<link rel="stylesheet" href="./css/main.css">
```
- Veuillez supprimer les chemins incohérents (`../css/main.css` et doublons)

## B) Mettre tous les `<link>` dans le `<head>`
- Vous avez un favicon :
  - placé en dehors du `<head>` (ce n’est pas correct)
- Veuillez placer tous les `<link rel="icon"...>` uniquement dans le `<head>`

## C) Structure de page : un seul `<header>` et un `<h1>` dans `<main>`
- Vous avez deux balises `<header>` : veuillez n’en garder qu’une seule
- Veuillez mettre le `h1` (votre nom + prénom) dans `<main>`
- Le `<header>` doit contenir : la photo + le menu

## D) Photo dans le header : cliquable et ouverture nouvel onglet
- Veuillez rendre la photo cliquable et ouvrir l’image dans un nouvel onglet
- Exemple :
```
<a href="./img/img.png" target="_blank" rel="noopener noreferrer">
  <img src="./img/img.png" alt="Photo de Prénom Nom">
</a>
```

## E) Corriger les `id` (pas d’accents, pas d’espaces, pas de majuscules)
- Vos `id` contiennent des accents/espaces/majuscules (ex: `Compétences`, `centres d'intérêt`)
- Veuillez utiliser des `id` simples :
  - `experience`
  - `competences`
  - `formation`
- Et mettre à jour le menu (`href="#..."`) pour correspondre

## F) Ajouter un `<footer>` avec copyright + e-mail cliquable
- Il manque le footer obligatoire
- Veuillez ajouter :
  - `&copy;2025`
  - votre e-mail en lien `mailto:`
- Exemple :
```
<footer>
  &copy;2025 Prénom Nom —
  <a href="mailto:prenom.nom@email.com">prenom.nom@email.com</a>
</footer>
```

## G) Corriger les liens externes (target + sécurité)
- Vous avez `target="blank"` : ce n’est pas correct
- Veuillez utiliser `target="_blank"` et ajouter `rel="noopener noreferrer"`

## Autres
- balise `<meta>` pour la description absente dans le `<head>`
