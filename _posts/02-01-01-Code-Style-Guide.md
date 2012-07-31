# Guide de Style de codage

La communauté PHP est vaste et diversifiée, composée de bibliothèques innombrables, de cadres de développement
(frameworks) et de composants. Il est commun pour les développeurs PHP de choisir plusieurs d'entre eux et de les
combiner en un seul projet. Il est donc important que le code PHP respecte autant que faire se peut, un style de codage
commun pour faciliter le travail des développeurs qui vont combiner et assortir différentes bibliothèques pour leurs
projets.

Le [Framework Interop Group][fig] (anciennement connu sous le nom de 'PHP Standards Group') a proposé et adopté une
série de recommandations de style, appelés [PSR-0][psr0], [PSR-1][psr1] and [PSR-2][psr2]. Ne vous laisser pas troubler
par ces noms. Ces recommandations sont tout simplement un ensemble de règles que certains projets tels que Drupal, Zend,
CakePHP, phpBB, AWS SDK, FuelPHP, Lithium, etc... ont commencé à adopter. Vous pouvez utiliser ces normes dans vos
propres projets ou continuer à utiliser votre propre style.

Idéalement, vous devriez écrire du code PHP conforme à une ou plusieurs de ces normes afin que les autres développeurs
puissent facilement lire et travailler avec votre code. Ces normes s'ajoutent ainsi utiliser PSR-1 implique de se
conformer à PSR-0, mais pas à PSR-2.

* [A lire au sujet de PSR-0][psr0]
* [A lire au sujet de PSR-1][psr1]
* [A lire au sujet de PSR-2][psr2]

Vous pouvez utiliser les outils de [phpcs-psr][phpcs-psr] pour [PHP_CodeSniffer][phpcs] afin de vérifier que le code est
conforme aux recommandations. Vous pouvez également utiliser [PHP Coding Standards Fixer][phpcsfixer] de Fabien Potencier
pour modifier automatiquement la syntaxe de votre code et donc le rendre conforme à ces normes, vous économisant du temps
et des efforts en ne réglant pas les problèmes à la main.

[fig]: http://www.php-fig.org/
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
[psr1]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md
[psr2]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md
[phpcs]: http://pear.php.net/package/PHP_CodeSniffer/
[phpcs-psr]: https://github.com/klaussilveira/phpcs-psr
[phpcsfixer]: http://cs.sensiolabs.org/
