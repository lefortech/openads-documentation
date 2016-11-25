#########
Ergonomie
#########

Tableau de bord
===============

Le tableau de bord est composé de plusieurs blocs d'informations appelés widget qui permettent à l'utilisateur de visualiser rapidement des informations transverses.

.. image:: tableau-de-bord-exemple.png

La disposition des widgets est propre à chaque profil et peut être modifiée très facilement par l'administrateur.


Widgets
=======

.. _widget_dossiers_limites:

Widget "Dossiers limites"
-------------------------

.. image:: widget_dossiers_limites.png

Orienté Instruction.

L'objet de ce widget est de présenter un listing des dix dossiers d'instruction qui sont tacites dont la date limite est dans moins de X jours (le nombre de jours est :ref:`paramétrable <administration_widget_dossiers_limites>` par l'administrateur). 

Trois filtres sont disponibles sur ce widget (le filtre est :ref:`paramétrable <administration_widget_dossiers_limites>` par l'administrateur) :

- filtre par instructeur : on présente uniquement les dossiers dont il est spécifiquement instructeur.
- filtre par division : on présente tous les dossiers de la division de l'instructeur.
- aucun filtre : tous les dossiers auxquels l'utilisateurs a accès (si l'utilisateur appartient à une commune niveau mono, alors l'utilisateur n'a accès qu'aux dossiers de sa commune et si l'utilisateur appartient à une commune multi, alors l'utilisateur a accès à tous les dossiers).

Par défaut, tous les types de dossiers apparaissent dans ce listing (les types sont :ref:`paramétrable <administration_widget_dossiers_limites>` par l'administrateur).

A tout moment, au survol de l'icône d'information du widget, une description permet d'indiquer quels sont les paramètres appliqués sur le widget.

Le listing présente les informations suivantes :

- le libellé du dossier d'instruction,
- le nom du pétitionnaire principal,
- la date limite,
- le caractère à enjeux du dossier.

Un lien sur chaque enregistrement permet d'accéder à la fiche de visualisation du dossier d'instruction.

Un lien "Voir +" permet d'accéder au listing des mêmes dossiers sans limite de nombre.


.. _widget_recherche_dossier:

Widget "Recherche Dossier"
--------------------------

.. image:: widget_recherche_dossier.png

Orienté Instruction.

Ce widget permet de rechercher un dossier, et d'y accéder directement depuis le tableau de bord. Si le code du dossier est saisi dans son intégralité et que le numéro de dossier n'est pas ambigu (s'il existe un seul dossier commencant par ce numéro), on accède directement à la fiche de visualisation du dossier d'instruction. Par contre si le numéro de dossier saisi n'est pas suffisamment explicite et que plusieurs résultats correspondent, alors on accède à un listing de dossiers d'instruction qui contiennent le numéro recherché (une recherche avancée permet alors d'affiner les résultats).

Exemples :

- Recherche du dossier PC 013055 0001 et il n'y a pas de dossier sur existant → Accès direct au dossier
- Recherche du dossier PC 013055 0002 mais le dossier PC 013055 0002M01 existe → Redirection vers la recherche car il y a 2 résultats.


.. _widget_consultation_retours:

Widget "Retours de Consultation"
--------------------------------

.. image:: widget_consultation_retours.png

Orienté Instruction.

L'objet de ce widget est d'alerter l'utilisateur sur le nombre de retours de consultation marqués comme 'non lu'. En effet, lorsque l'instructeur a créé une consultation sur un dossier, la réponse à la consultation peut se faire par plusieurs sources : le service consulté si celui ci a un compte sur openADS, la cellule suivi qui a pu recevoir le retour par courrier et le saisir lui-même ou un traitement automatique aui au bout du délai de consultation émet un retour tacite. Lorsque une de ces réponses à lieu alors la consultation est marquée comme 'non lu' pour que l'instructeur puisse en avoir connaissance et le nombre de ces consultations apparaît dans ce widget entouré d'un rond bleu.

Lorsqu'aucun retour de consultation n'est marqué comme 'non lu' alors un message l'indique à l'utilisateur.

Trois filtres sont disponibles sur ce widget (le filtre est :ref:`paramétrable <administration_widget_consultation_retours>` par l'administrateur) :

- filtre par instructeur : on présente uniquement les dossiers dont il est spécifiquement instructeur.
- filtre par division : on présente tous les dossiers de la division de l'instructeur.
- aucun filtre : tous les dossiers auxquels l'utilisateurs a accès (si l'utilisateur appartient à une commune niveau mono, alors l'utilisateur n'a accès qu'aux dossiers de sa commune et si l'utilisateur appartient à une commune multi, alors l'utilisateur a accès à tous les dossiers).

A tout moment, au survol de l'icône d'information du widget, une description permet d'indiquer quels sont les paramètres appliqués sur le widget.

Le menu d'openADS propose autant de listings que de filtres possibles : ainsi le lien "Voir +" redirige vers le tableau adéquat.


.. _widget_messages_retours:

Widget "Retours de Messages"
----------------------------

.. image:: widget_messages_retours.png

Orienté Instruction.

L'objet de ce widget est d'alerter l'utilisateur sur le nombre de messages marqués comme 'non lu'. En effet, lors de divers événements sur le dossier, des messages peuvent avertir l'instructeur qu'ils ont eu lieu (par exemple : l'ajout d'une pièce sur le dossier). Ce message est alors marqué comme 'non lu' pour que l'instructeur puisse en avoir connaissance et le nombre de ces messages apparaît dans ce widget entouré d'un rond bleu.

Lorsqu'aucun message n'est marqué comme 'non lu' alors un message l'indique à l'utilisateur.

Trois filtres sont disponibles sur ce widget (le filtre est :ref:`paramétrable <administration_widget_messages_retours>` par l'administrateur) :

- filtre par instructeur : on présente uniquement les dossiers dont il est spécifiquement instructeur.
- filtre par division : on présente tous les dossiers de la division de l'instructeur.
- aucun filtre : tous les dossiers auxquels l'utilisateurs a accès (si l'utilisateur appartient à une commune niveau mono, alors l'utilisateur n'a accès qu'aux dossiers de sa commune et si l'utilisateur appartient à une commune multi, alors l'utilisateur a accès à tous les dossiers).

A tout moment, au survol de l'icône d'information du widget, une description permet d'indiquer quels sont les paramètres appliqués sur le widget.

Le menu d'openADS propose autant de listings que de filtres possibles : ainsi le lien "Voir +" redirige vers le tableau adéquat.


.. _widget_nouvelle_demande_nouveau_dossier:

Widget "Nouvelle demande 'nouveau dossier'"
-------------------------------------------

.. image:: widget_nouvelle_demande_nouveau_dossier.png

Orienté Guichet.

Raccourci permet d'accéder directement au formulaire de saisie d'une nouvelle demande dans le cadre du dépôt d'un nouveau dossier.


.. _widget_nouvelle_demande_autre_dossier:

Widget "Nouvelle demande 'autres dossiers'"
-------------------------------------------

.. image:: widget_nouvelle_demande_autre_dossier.png

Orienté Guichet.

Raccourci permet d'accéder directement au formulaire de recherche d'un dossier en cours ou d'une autorisation existante pour y ajouter une nouvelle demande.


.. _widget_nouvelle_demande_dossier_encours:

Widget "Nouvelle demande 'dossiers en cours'"
---------------------------------------------

.. image:: widget_nouvelle_demande_dossier_encours.png

Orienté Guichet.

Raccourci permet d'accéder directement au formulaire de recherche d'un dossier en cours pour y ajouter une nouvelle demande.


.. _widget_dossiers_evenement_retour_finalise:

Widget "Dossiers auxquels on peut proposer une autre décision"
--------------------------------------------------------------

.. image:: widget_dossiers_evenement_retour_finalise.png

Ce widget liste les dossiers pour lesquels on peut proposer une autre décision.

Il s'agit de ceux dont le dernier événement d'instruction de type arrêté est finalisé,
n'est pas de type retour et ne dispose d'aucune date renseignée parmi les suivantes :

* date d'envoi pour signature ;
* date de retour de signature ;
* date d'envoi RAR ;
* date de retour RAR ;
* date d'envoi au contrôle légalité ;
* date de retour du contrôle de légalité.


.. _widget_dossiers_evenement_incomplet_majoration:

Widget "Dossiers événement incomplet ou majoration sans RAR"
------------------------------------------------------------

.. image:: widget_dossiers_evenement_incomplet_majoration.png

Orienté Instruction.

L'objet de ce widget est de présenter un listing de dix dossiers d'instruction maximum sur lesquels ont été appliqué un événement de majoration ou d'incomplétude avec une date d'envoi de lettre RAR renseignée pour cet événement, et dont la date de retour RAR de l'événement n'a pas été complétée. Les dossiers sont triés du plus récent au plus ancien.

Trois filtres sont disponibles sur ce widget (le filtre est :ref:`paramétrable <administration_widget_dossiers_evenement_incomplet_majoration>` par l'administrateur) :

- filtre par instructeur : on présente uniquement les dossiers dont il est spécifiquement instructeur.
- filtre par division : on présente tous les dossiers de la division de l'instructeur.
- aucun filtre : tous les dossiers auxquels l'utilisateurs a accès (si l'utilisateur appartient à une commune niveau mono, alors l'utilisateur n'a accès qu'aux dossiers de sa commune et si l'utilisateur appartient à une commune multi, alors l'utilisateur a accès à tous les dossiers).

A tout moment, au survol de l'icône d'information du widget, une description permet d'indiquer quels sont les paramètres appliqués sur le widget.

Le listing présente les informations suivantes :

- le libellé du dossier d'instruction,
- la date de dépôt du dossier,

Un lien sur chaque enregistrement permet d'accéder à la fiche de visualisation du dossier d'instruction.

Un lien "Voir tous les dossiers évènement incomplet ou majoration sans RAR" permet d'accéder au listing des mêmes dossiers sans limite de nombre.

Widget "Nouvelle demande 'nouveau dossier numérotation manuelle"
----------------------------------------------------------------

.. image:: widget_nouvelle_demande_nouveau_dossier_numerotation_manuelle.png

Orienté Guichet.

Raccourci permet d'accéder directement au formulaire de saisie d'une nouvelle demande dans le cadre du dépôt d'un nouveau dossier, avec la saisie manuelle du numéro de dossier.



Profils
=======

Administration
--------------

.. toctree::
    :maxdepth: 1
    
    profils/administrateur_general.rst
    profils/administrateur_technique_fonctionnel.rst

Visualisation
-------------

.. toctree::
    :maxdepth: 1
    
    profils/visualisation_da.rst
    profils/visualisation_da_di.rst

Instruction
-----------

.. toctree::
    :maxdepth: 1
    
    profils/chef_de_service.rst
    profils/divisionnaire.rst
    profils/instructeur.rst
    profils/instructeur_polyvalent.rst
    profils/instructeur_polyvalent_commune.rst
    profils/instructeur_service.rst
    profils/qualificateur.rst

Réception et suivi
------------------

.. toctree::
    :maxdepth: 1

    profils/suivi.rst
    profils/guichet_suivi.rst
    profils/guichet_unique.rst

Services consultés
------------------

.. toctree::
    :maxdepth: 1
    
    profils/service_consulte.rst
    profils/service_consulte_interne.rst
    
