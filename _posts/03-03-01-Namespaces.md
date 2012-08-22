---
isChild: true
---

## Espaces de nommage

Comme mentionné ci-dessus, la communauté PHP compte un grand nombre de développeurs qui crée une grande quantité de code source. Cela signifie qu'il est possible que deux bibliothèques utilisent un même nom de classe. Lorsque deux bibliothèques sont utilisées dans le même espace de nommage, cela peut provoquer une collision et donc causer des problèmes.

Les espaces de noms résolvent ce problème. Comme décrit dans le manuel de référence PHP, les espaces de nommage peuvent être comparés à _l'espace de nommage_ des fichiers dans les répertoires d'un système d'exploitation où deux fichiers portant le même nom peuvent coexister dans des répertoires distincts. De même, deux classes PHP avec le même nom peuvent coexister dans les espaces de noms PHP distincts. C'est aussi simple que cela.

Il est important de séparer votre code avec des espaces de nommage qui peuvent être utilisés par d'autres développeurs afin d'éviter les risques de collisions avec d'autres bibliothèques.

L'une des méthodes recommandée pour l'utilisation des espaces de noms est décrite dans [PSR-0][psr0] et vise à fournir une convention standard pour les fichiers, les classes et les espaces de noms, ce qui facilite l'échange et l'utilisation du code dans différents projets.

* [A lire au sujet des Espaces de noms][namespaces]
* [A lire au sujet PSR-0][psr0]

[namespaces]: http://php.net/manual/fr/language.namespaces.php
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
