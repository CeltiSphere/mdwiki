A Propos
=====

MDwiki est un CMS/Wiki __entièrement construit en HTML5/Javascript et fonctionnant 100% côté client__. Aucune installation de logiciel spécifique ou de processus serveur n'est requise. Il suffit juste de charger le fichier `mdwiki.html` fourni avec MDwiki dans le même répertoire que les fichiers markdown et tout est prêt !

Note: Le site web que vous consultez actuellement est realisé avec MDwiki et hébergé sur [GitHub pages](http://pages.github.com/). [http://mdwiki.info](http://mdwiki.info) redirige ici.

[gimmick:twitterfollow](timodoerr)

Caractéristiques
--------

  * Construit entièrement en Javascript/HTML5 et __ne nécessitant aucune installation locale ou à distance__
  * Utilise [Markdown][markdown] comme langage de saisie
  * Construit sur [jQuery][jQuery] et [Bootstrap3][bootstrap] pour fonctionner avec tous les navigateurs, avec un affichage responsive
  * Extensions de Markdown avec des [_Gimmicks_][gimmicks] specifiques qui enrichissent les fonctionnalités clients, comme la mise en forme de syntaxe par [hightlight.js][highlightjs], [GitHub Gists][gists], ou [Google Maps][maps] pour le geodata
  * Personnalisable avec une compatibilité Bootstrap, supporte tout thème issu de [bootswatch](http://www.bootswatch.com)


Requis
------------

* Espace web (ou un serveur web qui peut supporter des fichiers statiques)
* Un navigateur récent
* le fichier [mdwiki.html][download]

Comment ça fonctionne ?
-----------------

Déposer le fichier `mdwiki.html` récupéré sur [la page de téléchargment][download] avec vos fichiers en markdown sur un espace web. Vous pouvez passer n'importe quelle url (relative au fichier `mdwiki.html`) avec mdwiki après un hashbang `#!`:

    http://www.exemple.com/mdwiki.html#!monfichier.md

Si vous renommez le `mdwiki.html` en `index.html`, vous pouvez ommettre le nom du fichiers sur la plupart des serveurs web :

    http://www.exemple.com/#!monfichier.md

MDwiki chargera un fichier appelé `index.md` du même répertoire que le fichier index.html par défaut, donc si vous utilisez un fichier `index.md` comme point d'entrée, il vous suffit d'entrer votre nom de domaine :

    http://exemple.com/

Note: Découvrez les nombreuses fonctionnalités habituelles de Markdown sur le [tutoriel de démarrage][quickstart].

- - - -

Credits / Technologies
----------------------

MDwiki n'existerait pas sans une grande part de ces logiciels :

  * [marked][marked]
  * [jQuery][jQuery]
  * [Bootstrap][bootstrap]
  * [Bootswatch][bootswatch]
  * [colorbox][colorbox]
  * [highlightjs][highlightjs]

MDwiki est une création de Timo Dörr. Suivez-le pour connaître les mises à jour de MDwiki! [Follow @timodoerr](http://www.twitter.com/timodoerr).

Les jolies images de chatons proviennent de [placekitten.com].

  [Telechargement]: download.md
  [Demarrage]: quickstart.md
  [gimmicks]: gimmicks.md

  [markdown]: http://daringfireball.net/projects/markdown/
  [jQuery]: http://www.jquery.org
  [bootstrap]: http://www.getbootstrap.com
  [bootswatch]: http://www.bootswatch.com
  [marked]: https://github.com/chjj/marked
  [colorbox]: http://www.jacklmoore.com/colorbox/
  [gists]: https://gist.github.com/
  [maps]: http://maps.google.com/
  [highlightjs]: https://highlightjs.org/
  [placekitten.com]: http://www.placekitten.com/

License
-------

MDwiki est sous licence [GNU GPLv3 avec termes additionnels][license].

  [license]: https://github.com/Dynalon/mdwiki/blob/master/LICENSE.txt
