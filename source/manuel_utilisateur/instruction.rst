.. _instruction:

###########
Instruction
###########

=============================
Gestion des pièces du dossier
=============================

Chaque dossier d'instruction peut avoir plusieurs documents numérisés.

Ils sont listés dans l'onglet "Pièces" et organisés par date et catégorie des documents.

.. image:: piece_tab.png

Au clic sur le nom du document, il sera ouvert depuis le stockage au format PDF.

Pour ajouter un document il faut cliquer sur le "+" vert en haut de page à côtés de la mention "Ajouter un document".

.. image:: piece_form.png

Dans le formulaire qui apparaît tous les champs sont obligatoires :

* **Fichier** : Documents au format PDF à envoyer en GED.
* **Uid** : Documents au format PDF à envoyer dans le stockage.
* **Date de création** : Date de création du document.
* **Type de document** : Type du document.

===========================================
Documents numérisés ou reprise de l'arriéré
===========================================

Les documents numérisés ou repris doivent être placés dans le sous-dossier "Todo"
du dossier configuré dans la variable $config['path_scan'] (dyn/config.inc.php).

L'opérateur qui numérise les documents devra donc les déposer dans le sous dossier
nommé de la même façon que le dossier d'instruction lié.

Un service automatique se chargera de traiter ces documents : les enregistrer
dans le système de stockage prédéfini ainsi que les lier au dossier d'instruction
dans openADS. Les documents traités sont ensuite supprimés.

========================
Evenements d'instruction
========================

...

Compléments
===========

Il est possible d'ajouter des compléments d'informations pour les événements 
d'instruction depuis les blocs "Complément" et "Complément 2".

La plupart des compléments d'informations sont disponibles depuis la bible.

.. image:: instruction_complement_bible.png

Il suffit de choisir l'élément que l'on désire voir apparaître dans le champ 
complément.
En laissant la souris sur le libellé une infobulle affichera le texte qui sera 
affiché.

(Pour plus d'information sur la bible voir :ref:`parametrage_dossiers_bible`.)

.. _instruction_complement:

============
Finalisation
============

Finalisation des documents de l'instruction
===========================================

Pour finaliser l'édition de l'instruction, il faut cliquer sur le lien "Finaliser le document" du portail d'action de la visualisation.

.. image:: portlet_finaliser.png

Au clique sur le lien de l'édition dans le portail d'action de la visualisation de l'instruction, le document sera ouvert depuis le stockage au format PDF.

L'instruction n'est plus ni modifiable, ni supprimable.

Il est aussi possible de dé-finaliser le document au clique sur le lien "Reprendre la rédaction du document".

.. image:: portlet_definaliser.png

Lorsque le document est finalisé certaines informations concernant le dossier
lui sont associées lors de l'enregistrement.

Il est aussi possible de dé-finaliser le document au clique sur le lien "Reprendre la rédaction du document".

Le clique sur le lien de l'édition dans le portail d'action de la visualisation de l'instruction ouvrira le document généré à la volée au format PDF.

L'instruction est à nouveau modifiable et supprimable.


Finalisation des documents du rapport d'instruction
===================================================

Pour finaliser l'édition du rapport d'instruction, il faut cliquer sur le lien "Finaliser le document" du portail d'action de la visualisation.

.. image:: portlet_finaliser.png

Lorsque le document est finalisé certaines informations concernant le dossier
lui sont associées lors de l'enregistrement.

Au clique sur le lien de l'édition dans le portail d'action de la visualisation du rapport d'instruction, le document sera ouvert depuis le stockage au format PDF.

Le rapport d'instruction n'est plus ni modifiable, ni supprimable.

Il est aussi possible de dé-finaliser le document au clique sur le lien "Reprendre la rédaction du document".

.. image:: portlet_definaliser.png

Le clique sur le lien de l'édition dans le portail d'action de la visualisation du rapport d'instruction ouvrira le document généré à la volée au format PDF.

Le rapport d'instruction est à nouveau modifiable et supprimable.


Enregistrement de l'arrêté
==========================

Lors de la finalisation d'un évènement d'instruction de type arrêté le document
est enregistré sur le systeme de fichier.
Lorsqu'il revient après signature par l'autorité compétente, les informations qui
le compose sont envoyé au référentiel des arrêtés, et le document finalisé est
enregistré dans le systeme de fichiers associé à certaines informations (numéro 
de l'arrêté dans le référentiel, informations concernant le signataire, le terrain,
et l'arrêté).