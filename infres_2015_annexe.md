# Information annexes

## Git

Le projet doit etre posé sur github du commit 0 au dernier.
Chaque fonctionalité doit avoir sa 'branch'.
Chaque fonctionalité doit etre mergé sur master.
Les itérations doivent etre tagées (avec un git tag)

## Pull request

L'usage de [gitflow](http://danielkummer.github.io/git-flow-cheatsheet/) est plus que conseilé pour la création de branch (mais pas les merge)
Chaque merge de fonctionalité doit etre une pull request !!!

## Constitution des groupes

de 3 à 5 personnes par groupe (5 conseillé pour finir le sujet et mieux noté)

Chaque personne doit avoir effectué des commits en son nom (compte github) pour avoir une note.

## Ordre d'écriture 

Les fonctionalités peuvent etre réparties entre les membres du groupe librement, et effectuées dans l'ordre voulu.
Notament les 'chores' (implementation purement technique (lib d'upload, mail, auth))

**Toutefois il est important de respecter une chose !**

Les fonctionalités des itérations doivent etre effectuées dans l'ordre.
Il est interdit d'implémeter une fonctionalité d'itération n+1 (qui utiliserait des fichiers "controller, models, migration, views" d'itération n). 
Le sujet cherche en effet à vous faire des migrations et des modification de code et visualiser les changements dans les PR (pull request).

## Librairie et services utiles 

### Images 

Utiliser au choix

- [paperclip](https://github.com/thoughtbot/paperclip)
- [carrierwave](https://github.com/carrierwaveuploader/carrierwave)

Ou

- [cloudinary](http://cloudinary.com/)

Cloudinary peut se combiner avec l'un des deux.

### Mail

Utiliser au choix

- [sendgrid](https://sendgrid.com/)
- [mandrill](http://mandrill.com/)
- [postmarkapp](https://postmarkapp.com/)

(je suis curieux de mandrill mais si tout les groupes l'utilisent ce serait dommage)

### Deploys

Pour ceux qui voudraient jouer les malins vous pouvez tenter un deploy 
(ce qui serait impressionant mais pas nécessaire).

- [heroku](http://heroku.com)

Attention cloudinary est obligatoire (ou alors AS3)
et `assets:precompile` un problème à résoudre.

## Questions
Toute question sur le sujet, est à poser sous la forme une 'issue' dans github.

## Have fun
:)
