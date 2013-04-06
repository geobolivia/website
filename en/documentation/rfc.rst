.. _`georchestra.en.documentation.rfc`:

====================
RFC managment
====================

This section describes the operation of the RFC (Request For Comment * *). 
RFCs are formalized proposals in order to propose major changes to the geOrchestra project.
 
Examples of changes which can that are RFC subject (see below for detailed list) :

* major features ;
* code re-architecture ;
* community process improvements;
* intellectual property.
  
How it works ?
=========================
This is the RFC life cycle :

1. the developer intends to make a significant change ;
2. he communicates on the list (see :ref:`georchestra.en.community.index`) with community about changes ; 
   everyone can comment proposals on the list, but only the PSC members votes will be counted ;
3. the developer makes changes to the code ;
4. he writes an RFC detailing its changes and its consequences ;
5. the PSC vote RFC. Proposals must be available for review for at least two days before a final decision can be made. 
6. if the RFC is approved, the developer commits Code or patch necessary and make or change the documentation. 

Vote d'une RFC
===============
Le PSC a la charge de voter les RFC proposées par la communauté. Le processus de 
vote est le suivant :

* chaque membre du PSC possède un vote qui peut être -1 (rejet), -0, +0, +1 
  (acceptation) ;
* un membre du PSC qui vote négativemenet doit fournir un minimum d'explication ;
* un membre du PSC qui vote négativement doit proposer une solution de rechange 
  en un temps limité ;
* un vote de -0 indique un désaccord doux, mais n'a aucun effet. Le 0 indique 
  l'absence d'avis. Un +0 indiquent un appui doux, mais n'a aucun effet ;
* l'auteur de la RFC doit rédiger un minimum de retour dans sa proposition ;
* un vote négatif est analysé pour voir comment modifier le critère bloquant 
  pour obtenir un vote positif.
* la proposition est considérée comme acceptée après qu'une majorité absolue a 
  voté +1 et toutes les remarques sur les votes négatifs ont été résolues. 
  L'auteur de la proposition doit annoncer si celle-ci est acceptée 
  (proposition acceptée par la majorité des committers) ou s'il retire sa 
  proposition (veto). 

Le président dispose d'un vote. Il est chargé de maintenir à jour la liste des 
membres du PSC du projet. L'ajout et la suppression d'un membre au comité de 
pilotage, ainsi que la sélection d'un président doit être traitée comme une 
proposition au PSC. 

Le président statue dans les cas de litiges sur un vote.

Une proposition ne sera acceptée que si elle reçoit +2 (y compris l'auteur) et 
pas de veto (-1).

Si un veto est opposé à une proposition, et que celle-ci ne peut être revue 
pour satisfaire l'ensemble des votants, alors la proposition peut être soumise 
à un nouveau vote dans lequel une majorité de tous les votants éligibles 
indiquant +1 est suffisante pour l'adopter. Notez que c'est la majorité de tous 
les membres du PSC, et pas seulement ceux qui ont effectivement voté. 

Implémentation d'une RFC
===========================

Les RFC proposées, discutées et votées sont disponible dans la section `RFC dans
le wiki <http://csm-bretagne.fr/redmine/projects/georchestra/wiki/RFC>`_ de la 
forge.

Quand le vote est-il obligatoire ?
====================================

Le vote est obligatoire dans les cas suivants :

* Toute modification de la composition du comité (nouveaux membres, 
  suppression de membres inactifs) 
* Modifications au projet d'infrastructure (par exemple l'outil, l'emplacement 
  ou la configuration de fond) 
* Tout ce qui peut causer des problèmes de compatibilité descendante. 
* Ajout des quantités importantes de nouveau code. 
* Modification API inter-sous-système, ou des objets. 
* Les questions de procédure. 
* Lorsque une release doit avoir lieu. 
* Tout en matière de relations avec des entités extérieures telles que l'OSGeo.
* Tout ce qui pourrait être sujet à controverse.

