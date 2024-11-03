Structure du dossier de CakePHP
###############################

Après avoir téléchargé et extrait l'application CakePHP, voici les fichiers et
répertoires que vous devriez voir:

- Le dossier *bin* contient les exécutables de la console Cake.
- Le dossier *config* contient les (quelques) fichiers de
  :doc:`/development/configuration` que CakePHP utilise. Les détails sur la
  connexion à la base de données, le bootstrapping, les fichiers de
  configuration du cœur et consorts doivent être stockés ici.
- Le dossier *logs* contient normalement vos fichiers de log selon la
  configuration par défaut des logs.
- Le dossier *plugins* est l'endroit où sont stockés les :doc:`/plugins` que
  votre application utilise.
- Le dossier *src* sera celui vous placerez les fichiers source de votre application.
- Le dossier *templates* contient les fichiers de présentation :
  éléments, pages d'erreur, mises en page (layout) et les fichiers de vues.
- Le dossier *resources* contient un sous-dossier pour différents types de fichiers de
  ressources.
  Le sous-dossier *locales* stocke les fichiers de langue pour l'internationalisation.
- Le dossier *tests* est l'endroit où vous mettez les cas de test pour votre
  application.
- Le dossier *tmp* est l'endroit où CakePHP stocke les données temporaires. Les
  données qu'il stocke dépendent de la façon dont vous avez configuré CakePHP
  mais ce dossier est généralement utilisé pour les stocker les traductions,
  les descriptions de model et parfois les informations de session.
- Le dossier *vendor* est l'endroit où CakePHP et d'autres dépendances de
  l'application vont être installés par `Composer <https://getcomposer.org>`_.
  Modifier ces fichiers est déconseillé car composer écrasera vos changements
  lors du prochain update que vous ferez.
- Le répertoire *webroot* est la racine publique de votre application. Il
  contient tous les fichiers que vous souhaitez voir accessibles publiquement.

  Assurez-vous que les dossiers *tmp* et *logs* existent et qu'ils sont en
  écriture, autrement la performance de votre application sera sévèrement
  impactée. En mode debug, CakePHP vous avertira que ces dossiers ne peuvent
  pas être écrits.

Le Dossier Src
==============

Le répertoire *src* de CakePHP est l'endroit où vous réaliserez la majorité
du développement de votre application. Regardons d'un peu plus près les dossiers
à l'intérieur de *src*.

Command
    Contient les commandes de la console de votre application. Voir
    :doc:`/console-commands/commands` pour en savoir plus.
Console
    Contient le script d'installation exécuté par Composer.
Controller
    Contient les :doc:`/controllers` et les components de votre application.
Middleware
    Contient les :doc:`/controllers/middleware` de votre application.
Model
    Contient les tables, entity et behaviors de votre application.
Shell
    Contient les commandes de la console et les tasks de la console pour votre
    application. Pour plus d'informations, regardez la section
    :doc:`/console-commands/shells`.
View
    Les classes de présentation sont placés ici : views, cells, helpers.

.. note::

    Le dossier ``Shell`` n'est pas présent par défaut.
    Vous pouvez l'ajouter lorsque vous en avez besoin..

.. meta::
    :title lang=fr: Structure du dossier de CakePHP
    :keywords lang=fr: librairies internes,configuration du cœur,descriptions du model,librairies externes,détails de connexion,structure de dossier,librairies tierces,engagement personnel,connexion base de données,internationalisation,fichiersd e configuration,dossiers,développement de l'application,à lire,lib,configuré,logs,config,tierce partie,cakephp
