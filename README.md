# 🦝 Mockoon : les bouchons contre-attaquent !

![License](https://img.shields.io/badge/license-MIT-green)
![Reveal.js](https://img.shields.io/badge/reveal.js-4.5.0-yellow)
![Asciidoctor](https://img.shields.io/badge/asciidoctor-2.0-blue)

## 📝 Description

Ce dépôt présente l'ensemble des sources de la conférence `Mockoon : les bouchons contre attaquent !`
Découvrez comment simuler vos services web en quelques clics et accélérer votre développement.

L'article associé sur mon blog est disponible [ici](https://blog.hot-coffee.dev/blog/mockoon_conf/).

## 🚀 Générer les slides

### Installation

1. Clonez le dépôt :
```bash
git clone https://github.com/ibethus/mockoon-conf.git
cd mockoon-conf
```

2. Téléchargez Reveal.js :
```bash
wget https://github.com/hakimel/reveal.js/archive/master.zip
unzip master.zip -d slides
mv slides/reveal.js-master slides/reveal.js
rm master.zip
```

3. Générez les slides :
```bash
docker container run --rm \
  -u $(id -u):$(id -g) \
  -v $(pwd):/documents \
  asciidoctor/docker-asciidoctor:1.65 \
  asciidoctor-revealjs index.adoc
```

4. Ouvrez `index.html` dans votre navigateur !

## 🎮 Démo

La démo associée est disponible sur [ce dépôt](https://github.com/ibethus/mockoon-conf-demo).

## 📚 Documentation

- [Documentation Mockoon](https://mockoon.com/docs/latest/about/)
- [Guide Reveal.js](https://revealjs.com/)
- [Asciidoctor Reveal.js](https://docs.asciidoctor.org/reveal.js-converter/latest/)
- La palette de couleur est générée grâce à https://www.figma.com/color-palette-generator/

## 📝 License

Ce projet est sous licence MIT - voir le fichier [LICENSE](./LICENSE.md) pour plus de détails.