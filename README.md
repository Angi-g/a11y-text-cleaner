# a11y-text-cleaner
extension chrome / mozilla qui vise à rendre accessible les posts de réseaux social qui sont rédigés avec des caractères fantaisiste (unicode décoratif, alphabet mathématique, etc...),
L'utilisateurice pourra choisir
- masquer les posts (remplassé par un message d'avertisssement, avec option de pouvoir l'afficher quand même si iels souhaitent) 
- traduire avec du vrai texte, lisible et accessible, et le formatage qui était souhaité (gras, italique...)

plus d'info sur ce que sont ces char fantaisiste : 
vidéo de Julie Moynat:
- https://www.youtube.com/watch?v=OO1G70if4RU

Ou sa transcription textuelle en article : 
- https://www.lalutineduweb.fr/detournement-unicode-emojis-accessibilite/

## Etat
- POC pas commencé, des décisions technique a prendre pour commencer
- 1ere cible : linkedin

## Roadmap écrite a l'arache et a améliorer
- [ ] reconnaissance des char farfelu
- [ ] mode masquage : on remplace les posts qui ont des caractère fantaisiste par le texte "ce post de ( nom ou psoeudo de l'utilisateurice ) contiens des caractère illisible par les outiles d'accessibilité"
- [ ] ajouter l'option "afficher ce post malgrès tout" sur les posts masqué
- [ ] ajouter une option pour qu'une pop up s'affiche pour valider le fait qu'on veut interragir avec un post qui contien des char fantaisiste (objectif : inciter a limiter la visibilité de ces posts)
- [ ] traduire les textes en texte lisible et accessible
- [ ] nice to have : les formater avec du html pour qu'ils aient la forme que souhaitaient la personne qui post (le faux gras en <b>, etc...)
- [ ] parametre utilisateurice : pouvoir choisir entre masquer, masquer avec option d'afficher, traduction direct, message de popup pour inciter a pas promouvoir le post
- [ ] integration multi-site (linkedin, mastodon, bluesky, insta, autre...)
- [ ] bien tester les devs avec des lecteurs d'écran, et probablement faire un tableau pour dire quelle fonctionalité a été testé avec quel lecteur d'écran, et fonctionne

## Sécurité et vie privé
- l'extension doit pouvoir fonctionner coté client sans aucun envoi réseau, et aucun tracking
- pas d'innerHTML, pas d'execution de code externe

## Contribuer
C'est la 1ere fois que je fais un projet pour l'exterieur et que je veux open source, AIDEZ MOI
- vous pouvez ouvrir des issues (bug, mapping manquant, idées).
- vous pouvez faire des PRs si vous voulez contribuer au code ou a la doc
