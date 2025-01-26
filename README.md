# Mockoon : les bouchons contre-attaquent !

## Description
Ce dépôt présente l'ensemble des sources de la conférence `Mockoon : les bouchons contre attaquent !`

## Générer les slides en local

1. Télécharger `reveal.js`, le dézipper dans le répertoire `slides` et nommer le répertoire `reveal.js` : https://github.com/hakimel/reveal.js/archive/master.zip


2. Lancer les commandes suivantes :
```
docker container run --rm -u $(id -u):$(id -g) -v $(pwd):/documents asciidoctor/docker-asciidoctor:1.65 asciidoctor-revealjs index.adoc
```

3. Ouvrir le fichier index.html généré.