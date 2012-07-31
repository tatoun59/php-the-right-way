---
isChild: true
---

## Configuration Windows

PHP est disponible de différentes manières sous Windows. Vous pouvez [télécharger les binaires](php-downloads) et
jusqu'à récemment, vous pouviez utiliser un fichier d'installation .msi. Le programme d'installation n'est plus supporté
et s'arrête à PHP 5.3.0.

Pour l'apprentissage et le développement local, vous pouvez utiliser le serveur web intégré à PHP 5.4 sans vous soucier
de sa configuration. Si vous souhaitez une solution "tout-en-un" qui comprend un serveur web à part entière et MySQL 
alors des outils tels que le [Web Platform Installer] [wpi], [Zend Server CE] [zsce], [XAMPP] [xampp] et [WAMP] [wamp]
vous aideront à obtenir rapidement un environnement de développement sous Windows. Cela dit, ces outils seront
un peu différents de ceux rencontrés en production. Soyez donc attentif sur les différences d'environnement lorsque vous
travaillez sous Windows et déployez ensuite sous Linux.

Si votre système de production doit fonctionner sous Windows alors le serveur IIS sur Windows 7 fournira de meilleures
performances et une plus grande stabilité. Un outil tel que [Phpmanager][phpmanager] (plugin graphique pour IIS 7)
permettra de simplifier la gestion et la configuration de PHP sur ce serveur. IIS 7 embarquant FastCGI est configuré et
prêt à l'emploi. Il suffit de pointer vers PHP en tant que contrôleur. Pour plus d'informations et des ressources
supplémentaires, se référer à [l'espace dédié sur iis.net][php-iis] à PHP.


Generally running your application on different environment in development and production can lead to strange bugs popping up when you go 
live. If you are developing on Windows and deploying to Linux (or anything non-Windows) then you should consider using a Virtual Machine. This 
sounds tricky, but using [Vagrant][vagrant] you can set up simple wrappers, then using [Puppet][puppet] or [Chef][chef] you can provision these boxes and share them with your colleagues to ensure you're all working on the same stack. More on this soon.

En général d'exécuter votre application sur l'environnement différent dans le développement et la production peut conduire à des bugs étranges surgissent quand vous allez
vivre. Si vous développez sur Windows et le déploiement de Linux (ou n'importe quoi non-Windows), alors vous devriez envisager d'utiliser une machine virtuelle. cette
sonne délicate, mais en utilisant [Vagrant] [vagabond], vous pouvez mettre en place des wrappers simples, puis en utilisant [marionnettes] [marionnettes] ou [chef] [chef] vous pouvez fournir ces boîtes et de les partager avec vos collègues pour vous assurer que vous êtes tous travail sur la même pile. Plus à ce sujet bientôt.

En général, exécuter une application dans des environnements différents en développement et en production peut conduire
à des bugs étranges lors de son utilisation. Si vous développez sur Windows et déployez sur Linux (ou tout système autre
que Windows), vous devriez envisager d'utiliser une machine virtuelle. Cela peut sembler un peu compliqué, mais en
utilisant de simples conteneurs [Vagrant][vagrant], puis en utilisant [Puppet][puppet] ou [Chef][chef], vous pouvez 
fournir et partager des plateformes avec vos collègues, qui assureront un environnement de travail homogène.
Plus sur ce sujet ultérieurement.

[php-downloads]: http://windows.php.net
[phpmanager]: http://phpmanager.codeplex.com/
[wpi]: http://www.microsoft.com/web/downloads/platform.aspx
[zsce]: http://www.zend.com/fr/products/server-ce/
[xampp]: http://www.apachefriends.org/fr/xampp.html
[wamp]: http://www.wampserver.com/
[php-iis]: http://php.iis.net/
[vagrant]: http://vagrantup.com/
[puppet]: http://www.puppetlabs.com/
[chef]: http://www.opscode.com/
