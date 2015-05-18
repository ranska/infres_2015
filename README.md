# Sujet de projet ruby on rails
Un bon sujet d'application ruby on rails est un sujet qui met en valeur les qualités de rails.

A savoir, la facilité de changement qui permet à une petite startup d'etre agile.

*Ainsi donc ce sujet simule l'évolution d'une application dans le temps.*

## Action attendue pour la notation
Pour chaque question il doit y avoir: 
1. un 'commit' 
2. une 'branch'
3. et en vue de la présentation finale une capture d'écran 
  permettant au jury de comprendre les évolutions (changements graphiques ou fonctionels)

# Sncf réclamation.

# Itération 0 
_le P.O.C en starup weekend_

## pitch:
Féderer les personnes ayant des réclamantions à faire
dans le but de grouper les réclamations et peser davantage.

*Un porteur de projet vient vous voir pour faire son projet*

## Fonctionalité principale 
```Cucumber
En tant que "utilisateur" du service 
Lorsque je suis dans mon espace
Alors je peux créer un réclamation
Et uploader une preuve de consommation (image de ticket)
Et uploader une ou plusieurs preuves de dysfonctionement
Et remplir une description
Alors la réclamation est publiée
```

Lors de cette itération implementez:
1. Une page home avec l'index des réclamations
1. Un espace authentifié ou chaque utilisateur peut 'CRUD' ses publications


# Itération 1 
_Quelques soirs et week-ends après_

*Le porteur de projet veut allez plus loin, il vous achète des préstat*
*Il s'appelle désormais "le client"*

1. Un admin peut supprimer un message désobligeant
1. Chaque réclamation est un groupe
1. Un utilisateur peut rajouter sa participation à une réclamation # ou toujours créer sa propre réclamation

# Itération 2
*Le P.O.C commence à prendre forme avec les eurly-adopters*

Pour éviter les messages désagréables le client veut de la modération
Pour l'instant l'admin et le modérateur sont le meme acteur

1. Les réclamations ont un état (brouillon, publiè)
```cucumber
Alors la réclamation et dans mes brouillons
```
## Modération

1. Lorsque une réclamation est créée
   Un utilisateur peut publier une réclamation

2. Un moderateur peut demander l'amélioration d'une réclamation
   la réclamation n'est plus visible
   et le système notifie "l'utilisateur" avec un message # message de rejet ou d'indication

3. Un moderateur peut refuser définitivement une réclamation

4. Un utilisateur peut soumetre à nouveau une réclamation refusée

### Woops

Le client ne vous l'avait pas dit car 'dans ma tete c'était implicite'
Bien évidement la modération implique maintenant 2 concepts 'réclamation' et 'participation à réclamation'
(comme vous avez lu ce sujet en entier, (c'est un peu comme si vous etiez un pro,
qui pose les bonnes questions au bon moment.) Proposez directement quelque chose qui tient la route)

# Itération 3 
*ça y est c'est la béta*

On va peser dans la place il faut maintenant communiquer vers l'extérieur.
Le client à plein d'idées de fou (API, mail de PDF pour la presse, génération de GIF annimé,
twitter facebook et autre!!!)

## Une première fonction réalise
Un mail est envoyé automatiquement lorsque la réclamation atteind 10 personnes.

## Une première modification
Le client arrete pas de parler de facebook et que 10 personnes c'est nul,
vous tenez bon et lui faites une 1ère proposition.

### quelques aller retours
(pour chaque étape faites un commit)

1. le système envoie une réclamation (sous forme de mail, à la sncf) 30 jours
   après sa création.

*le client va partir en vacances (et veut voir de l'activité sur son site)*

1. Avant 30 jours une réclamation est envoyée si il y a déjà 100 personnes

*Le client est bronzé et motivé*

1. Le modérateur peut surcharger la condition d'envoi de mail 
ou déclancher l'envoi lui meme. (changer le nombre de jours ou nombre personnes)

(le choix ou non de faire un 'model' 'Condition' est pour vous, 
de toute façon le client 
'y y connais ruien à l'formatiqueu')
 
# Itération 4 
*Il est temps de faire venir la foule*

Le client n'a plus trop d'argent alors après grosse négo, (si si tu peux le faire)
vous évaluez la possiblilité de faire des post tweeter ou facebook automatiques.
## évaluer 

Quelles fonctionnalités préalables, quelles lib, gem utiliser, quelle doc.

## chiffrer 

Planning pocker basé sur votre expérience du projet, photo de la séance, si
vous n'avez pas de carte trouvez un moyen

## Implémenter

Vous avez évalué et comme par hasard le client pose de l'argent frais sur la table.

# Itération 5 
*1ère grosse traction*

Enfin en théorie, un investisseur privé repose de l'argent sur la table.
Le but: revendre le service à l'un des gros acteur qui reçoit vos réclamations.

## Nouvelle feature

### Un super Admin 

1. Peut bloquer la publication
2. Peut réécrire les messages des users

3. Un onglet Stat super admin

4. Peut indiquer quel utilisateur réclame le plus
5. Quelle période de l'année il y a le plus de réclamations

#Partie bonus
### Comme aux éléctions

Les utilisateurs 

1. ont maitenant la possibilité de donner une note de gravité (0-5) à leur
réclamation.

Super Admin

1. Créer une participation sans pièce justificative
2. avec une note moyenne des autres participations -1
3. et un commentaire prérempli séléctionable

Stagiaire

1. Peut créer éditer une liste de commentaires préremplie

# Itération 6 
*Une fin avec de la morale*

La maman du client (une ex 68) corrige son rejeton et trouve un autre investisseur
plus moral.

Le service va se vendre en marque blanche pour chacun des grand acteurs du
transport.

avec des réclamations blanches (pour dumper sans cheater)

seuls les réclamants peuvent éditer leurs messages.


