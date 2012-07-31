---
isChild: true
---

## Configuration Mac

Le système OSX est préconfiguré avec un PHP qui est généralement une version légérement plus ancienne que la dernière
version stable. Le système Lion intégre PHP 5.3.6 et le système Mountain Lion comprend la version 5.3.10.

La mise à jour de PHP sur le système OSX peut être installé à l'aide de différents [gestionnaires de paquets][mac-package-managers].
Cependant, nous recommandons le paquet [php-osx by Liip][php-osx-downloads].

Une autre option est de [le compiler vous-même][mac-compile]. Dans ce cas, assurez-vous d'avoir installé l'application
de développement Xcode, ou à défaut, les ["Outils de ligne de commande pour Xcode"][apple-developer] téléchargeables
à partir du Centre d'Apple Mac Developer.

Enfin, si vous souhaitez avoir un paquet "Tout en un" comprenant PHP, le serveur web Apache, le gestionnaire de base
de données MySQL et une interface graphique de contrôle simple, vous pouvez essayer [MAMP][mamp-downloads].

[mac-package-managers]: http://www.php.net/manual/fr/install.macosx.packages.php
[mac-compile]: http://www.php.net/manual/fr/install.macosx.compile.php
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
[apple-developer]: https://developer.apple.com/downloads
[mamp-downloads]: http://www.mamp.info/en/downloads/index.html
[php-osx-downloads]: http://php-osx.liip.ch/
