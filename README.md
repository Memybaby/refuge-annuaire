# Refuge Animalier — annuaire d'urgence pour animaux (Québec)

## Ce qui est prêt
- `index.html` — page d'accueil (recherche par service + ville, 4 villes de lancement)
- `veterinaire-urgence-montreal.html` — page modèle avec 2 fiches **EXEMPLE** (à remplacer par de vraies cliniques)
- `style.css` — tout le style du site

Site 100% statique — aucun serveur, aucune installation, aucun coût. Il fonctionne directement quand il est déployé.

## Mettre le site en ligne (gratuit)
1. Sur GitHub mobile : crée un nouveau repository (ex. `refuge-annuaire`), et téléverse les 3 fichiers ci-dessus.
2. Va sur vercel.com, connecte ton compte GitHub, importe ce repository.
3. Vercel détecte que c'est un site statique — clique "Deploy". Aucune configuration nécessaire.
4. Tu obtiens une URL gratuite du type `refuge-annuaire.vercel.app` immédiatement utilisable.

## Prochaine étape : remplacer les exemples
Dans `veterinaire-urgence-montreal.html`, chaque bloc marqué **[EXEMPLE]** doit être remplacé par une vraie clinique :
- Nom, adresse, horaires réels, numéro de téléphone
- Le lien `tel:` doit contenir le vrai numéro
- Le bloc `Schema.org` en bas du fichier doit lui aussi être mis à jour (c'est ce qui aide Google à afficher des infos enrichies)

Dis-moi les vraies cliniques (nom, ville, téléphone, horaires) et je te génère les fiches — c'est plus rapide que de les écrire toi-même en HTML.

## Ajouter une nouvelle ville ou un nouveau service
On duplique `veterinaire-urgence-montreal.html` en changeant le nom de fichier (ex. `veterinaire-urgence-quebec.html`, `toiletteur-mobile-montreal.html`) et on ajoute le lien correspondant dans `index.html`. Dis-moi simplement quelle ville/service ajouter et je m'en occupe.

## Plus tard : base de données (quand il y aura beaucoup de fiches)
Tant que chaque ville a moins de 20-30 fiches, le HTML statique reste le plus simple et le plus rapide. Quand ce sera plus lourd à gérer à la main, on migrera vers Supabase (gratuit) pour gérer les fiches et les avis depuis une interface au lieu de fichiers HTML — mais ce n'est pas nécessaire pour lancer.
