<!-- LTeX: language=fr -->

InsTAL party
============

[![Licence : CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/)

Code pour générer le site de l'install party PluriTAL.

## Générer le site en local

Dépendances

- Ruby w/ bundle

Setup:

```console
gem install jekyll bundler
bundle config set --local path 'vendor/bundle'
bundle install
```

Régénérer

```bash
bundle exec jekyll build
bundle exec jekyll serve
```

(l'étape build n'est à proprement parler nécessaire que si tu as modifié `_config`)

## Changer les choses (avec des bouquets de roses)

### Modifier la page principale

C'est dans `index.md`, changes-y ce que tu veux.

### Ajouter des pages

Jekyll n'est pas très bon pour les pages qui ne sont pas des postes de blog. Si tu veux des
nouvelles pages, il faut les ajouter dans `_pages` (ce qui fonctionne parce qu'on l'a mis dans
`_config.yml`)- et leur donner un `permalink` dans le header.

### Changer le style

- Pour les couleurs, la typo… ça se passe dans `assets/css`.
- Pour la structure des pages, il faut regarder du côté de `_layouts` et `_includes`.
  - Lis bien la doc de Jekyll et regarde comment est construit [le thème
    parent](https://github.com/pages-themes/primer).
  - L'idée c'est que les fichiers dans **ce** repo ici que tu es en train de regarder remplacent
    ceux du thème parent, donc si tu veux customiser un fichier du thème parent, tu le copie-colle
    ici avec le même nom et le même chemin et tu y modifie ce que tu veux.

## Licences

[![CC BY Licence
badge](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

Copyright © 2022 Loïc Grobol [\<loic.grobol@gmail.com\>](mailto:loic.grobol@gmail.com)

Sauf indication contraire, les fichiers présents dans ce dépôt sont distribués selon les termes de
la licence [Creative Commons Attribution 4.0
International](https://creativecommons.org/licenses/by/4.0/).

Un résumé simplifié de cette licence est disponible à
<https://creativecommons.org/licenses/by/4.0/>.

Le texte intégral de cette licence est disponible à
<https://creativecommons.org/licenses/by/4.0/legalcode>