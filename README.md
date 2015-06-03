MISC : Introduction au développement d'extensions Burp, Exemple XSRF
====================================================================

Description
-----------
Ce dépôt contient les sources et binaires mentionnés dans l'article MISC.
 * La librairie Java `Jython` permet d'utiliser un script écrit en Python comme extension de Burp.
 * Le dossier `extension` contient le script permettant de modifier le paramète XSRF des requêtes HTTP ciblées.
 * Le dossier `server` contient un serveur d'exemple afin de tester l'extension.

Afin de lancer le serveur, la librairie Python `Flask` est nécessaire. Il est possible de l'installer à l'aide de l'utilitaire `pip` :

````
pip install -r requirements.txt
```

Copyright et licence
---------------------
Toutes les ressources de ce dépôt sont distribuées sous licence GPLv3.

Crédits
-------
* Vincent Dépériers
* Thomas Debize
