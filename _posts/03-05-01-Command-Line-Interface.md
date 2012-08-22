---
isChild: true
---

## L'interface de la ligne de commande
 
PHP a été créé principalement pour développer des applications Web, mais il est également très utile pour la mise en œuvre de programmes qui s'exécutent sur l'interface de ligne de commande (CLI). Les programmes en ligne de commande de PHP peuvent vous aider à automatiser les tâches courantes telles que les essais, le déploiement et la gestion d'applications.

Les programmes PHP CLI sont très puissants parce que le code de l'application peut être utilisé directement sans avoir à créer et sécuriser une interface web. Pour cette raison, il ne faut  pas déposer des programmes CLI à la racine publique de son site web !

Essayez de lancer l'instruction PHP suivante en ligne de commande :

{% highlight bash %}
> php -i
{% endhighlight %}

L'option `-i` affichera votre configuration PHP à l'identique de la fonction [`phpinfo`][phpinfo].

L'option `-a` appelle une console interactive similaire à l'IRS de Ruby ou la console de Python. Il existe plusieurs [options de ligne de commande][cli-options] qui sont très utiles. 

Nous allons écrire un programme simple qui affiche "Bonjour, $name" à la ligne de commande. 
Pour commencer, nous allons créer une archive `hello.php`, comme indiqué ci-dessous:

{% highlight php %}
<?php
if($argc != 2) {
    echo "Usage: php hello.php [name].\n";
    exit(1);
}
$name = $argv[1];
echo "Hello, $name\n";
{% endhighlight %}

PHP définit deux variables spéciales basées sur les arguments reçus par votre script lors de son exécution. [`$argc`][argc] est une variable de type entier contenant le *nombre d'arguments* et [`$argv`][argv] est une variable de type tableau contenant la *valeur* de chaque argument. Le premier argument est toujours le nom de votre fichier de script PHP, soit `hello.php` dans notre cas.

La expression `exit()` peut être utilisée avec un nombre différent de zéro pour vous faire savoir que la console de commande a échoué. Vous trouverez [ici][exit-codes], les codes de sortie les plus couramment utilisés.

Exécutez le script ci-dessous dans un terminal :

{% highlight bash %}
> php hello.php
Usage: php hello.php [name]
> php hello.php world
Hello, world
{% endhighlight %}


 * [En savoir plus sur l'usage de PHP en ligne de commande][php-cli]
 * [En savoir plus sur la configuration de Windows pour exécuter PHP en ligne de commande][php-cli-windows]

[phpinfo]: http://php.net/manual/fr/function.phpinfo.php
[cli-options]: http://www.php.net/manual/fr/features.commandline.options.php
[argc]: http://php.net/manual/fr/reserved.variables.argc.php
[argv]: http://php.net/manual/fr/reserved.variables.argv.php
[php-cli]: http://php.net/manual/fr/features.commandline.php
[php-cli-windows]: http://www.php.net/manual/fr/install.windows.commandline.php
[exit-codes]: http://www.gsp.com/cgi-bin/man.cgi?section=3&topic=sysexits
