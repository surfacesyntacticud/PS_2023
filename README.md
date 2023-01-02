# ParisStories_2023

Ce repository contient les fichiers produits automatiquement sur les données `ParisStories 2023`.
Le répertoire `rewrite` est destiné à contenir des fichiers de règles [Grew](https://grew.fr) qui peuvent être appliquées au corpus.

## Grew-match
Le corpus initial est disponible dans [Grew-match](http://universal.grew.fr/?corpus=SUD_PS_2023@latest).

La production du corpus transformé peut être automatisée et le corpus produit est ensuite disponible dans Grew-match.
Par exemple, le fichier [`test.grs`](rewrite/test.grs) contient une règle de correction et le résultat du corpus produit par cette règle est disponible dans [Grew-match](http://universal.grew.fr/?corpus=SUD_PS_2023@@test).

## Grew-web
L'outil [`Grew-web`](http://transform.grew.fr/) permet de développer et de tester des fichiers de réécriture.

On peut également construire une URL avec des arguments pour accéder directement aux données de GitHub dans `Grew-web`.
Par exemple, on peut accéder au fichier `ParisStories_2023_lePouvoirDesMots.conllu` et au fichier de règle `test.grs` avec l'URL:
http://transform.grew.fr?corpus=https://raw.githubusercontent.com/surfacesyntacticud/PS_2023/main/ParisStories_2023_lePouvoirDesMots.conllu&grs=https://raw.githubusercontent.com/surfacesyntacticud/PS_2023/main/rewrite/test.grs.

Il est conseillé de bien tester le fichier de règles dans `Grew-web` (et notamment de d'assurer qu'il n'y a pas d'erreur de syntaxe) avant de mettre à jour dans GitHub.

Pour produire automatiquement à partir d'autres fichiers de règles, merci de mettre un ticket dans les [issues](https://github.com/surfacesyntacticud/PS_2023/issues).
