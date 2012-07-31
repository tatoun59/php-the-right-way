---
isChild: true
---

## paradigmes de programmation

PHP est un langage flexible et dynamique qui supporte variétés de techniques de programmation. Il a considérablement
évolué au cours des années, notamment grâce à l'ajout d'un solide modèle de programmation orientée objet dans PHP 5.0
(2004), des fonctions anonymes et des espaces de nommage dans PHP 5.3 (2009), et les traits en PHP 5.4 (2012).

### Programmation orientée objet

PHP dispose d'un ensemble très complet de fonctionnalités de programmation orientée objet, comprenant le support des
classes, des classes abstraites, des interfaces, de l'héritage, des constructeurs, du clonage d'objet, des
exceptions et plus encore.

* [A lire au sujet de la Programmation Orientée Objet en PHP][oop]
* [A lire au sujet des Traits][traits]

### programmation fonctionnelle

PHP a la possibilité de déclarer des fonctions de première classe, ce qui signifie qu'une fonction peut être affectée
à une variable. Les fonctions définies par l'utilisateur comme celles propres au langage, peuvent être référencées
par une variable et invoquées dynamiquement. Les fonctions peuvent être passées comme arguments à d'autres fonctions
(fonction appelée fonctions d'ordre supérieur) et une fonction peut retourner d'autres fonctions.

La récursivité, qui est la possiblité donnée à une fonction de s'appeler elle-même, est supportée par le langage. 
Toutefois, le code PHP est plus axé sur l'itération.

Les fonctions anonymes (avec le support des closures) sont présents depuis PHP 5.3 (2009).

PHP 5.4 ajoute la capacité de lier des closures à la portée d'un objet et l'amélioration du support des fonctions de
type appelables de telle sorte qu'elles peuvent être utilisées de façon interchangeable avec des fonctions anonymes
dans presque tous les cas.

* Continuer la lecture sur [la programmation fonctionnelle en PHP](/pages/Functional-Programming.html)
* [A lire au sujet des fonctions anonymes][anonymous-functions]
* [A lire au sujet de la classe Closure][closure-class]
* [Plus de détails sur les Closures RFC][closures-rfc]
* [A lire au sujet des fonctions appelables][callables]
* [A lire au sujet des fonctions dynamiquement invoquées avec `call_user_func_array`][call-user-func-array]

### Meta programmation

PHP supporte des formes variées de méta programmation à travers des mécanismes tels que l'API Reflection et les 
Méthodes magiques. Il existe de nombreuses méthodes magiques comme `__get()`, `__set()`, `__clone()`, `__toString()`,
 `__invoke()`, etc qui permettent aux développeurs de se connecter au bon fonctionnement de la classe. Souvent, 
les développeurs Ruby disent que PHP n'a pas de fonctions `method_missing`, cependant ces aspects sont disponibles dans
 `__call()` et `__callStatic()`.

* [A lire au sujet des Méthodes Magiques][magic-methods]
* [A lire au sujet de Reflection][reflection]

[namespaces]: http://php.net/manual/fr/language.namespaces.php
[overloading]: http://uk.php.net/manual/fr/language.oop5.overloading.php
[oop]: http://www.php.net/manual/fr/language.oop5.php
[anonymous-functions]: http://www.php.net/manual/fr/functions.anonymous.php
[closure-class]: http://php.net/manual/fr/class.closure.php
[callables]: http://php.net/manual/fr/language.types.callable.php
[magic-methods]: http://php.net/manual/fr/language.oop5.magic.php
[reflection]: http://www.php.net/manual/fr/intro.reflection.php
[traits]: http://fr.php.net/manual/fr/language.oop5.traits.php
[call-user-func-array]: http://php.net/manual/fr/function.call-user-func-array.php
[closures-rfc]: https://wiki.php.net/rfc/closures
