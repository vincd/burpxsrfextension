MISC XX Introduction au développement d'extensions Burp - Exemple token XSRF
==================================================================================

Description
-----------
Ce dépôt contient les sources et binaires de l'extension Burp "token XSRF" décrite dans l'article "Introduction au développement d'extensions Burp" du MISC n°XX.  
Les ressources sont regroupées ainsi :
```
+---xsrf.py				: Le code Jython de l'extension
|
+---server				: Un exemple d'application Web requérant un paramètre XSRF unique à chaque requête
```


Usage
-----
### Extension
0. Sélectionner le chemin vers l'interpréteur Jython au sein de Burp ; 
1. Charger l'extension `xsrf.py` au sein de l'onglet `Extender` : aucun onglet n'apparait, les requêtes sont automatiquement modifiées à la volée.

### Exemple d'application Web
0. Démarrer le serveur Web `cd server && python server.py`
1. Visiter l'URL `http://localhost:8001`

Dépendances
-----------
### Pour l'extension
* La bibliothèque `Jython`, téléchargeable [ici](http://search.maven.org/remotecontent?filepath=org/python/jython-standalone/2.7.0/jython-standalone-2.7.0.jar)

### Pour l'exemple d'application Web
* La bibliothèque `Flask` et les différentes dépendances Python, installables avec `pip install -r requirements.txt`


Copyright et licence
---------------------
Toutes les ressources de ce dépôt sont distribuées sous licence GPLv3.


Crédits
-------
* Vincent Dépériers
* Thomas Debize
