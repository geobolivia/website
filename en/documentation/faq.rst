.. _`georchestra.en.documentation.faq`:

=======
F.A.Q.
=======

.. contents:: Summary
  :local:

Governance
============

What is the PSC (Project Steering Committee) ?
----------------------------------------------

The PSC is the project office: it decides the broad guidelines of the project, solves problems (technical or not). 
It is composed of the major contributors to the community.

Its members are elected by project "commmitters" (see document 
:ref:`georchestra.en.documentation.psc` fro more information).

How to contact the PSC (Project Steering Committee) ?
-----------------------------------------------------

Its contact is : psc at georchestra point org.

How to get an acces to the forge ?
----------------------------------

Site tracking developments geOrchestra is open to anyone interested in the project and its roadmap.

In the current phase of development and to the delivery of version stable, you can be informed in real time: announcements, submissions bugs, source code changes, recipe ...

To access all the resources, three steps :

1. rendez-vous sur http://applis-bretagne.fr/redmine/account/register pour 
vous enregistrer sur la plate-forme avec l'identifiant et l'adresse de 
messagerie de votre choix
2. contactez les administrateurs du projet geOrchestra sur info@georchestra.org 
en rappelant votre identifiant, afin qu'il valide votre inscription au projet.
3. une fois la confirmation reçue par messagerie, rendez-vous sur 
http://applis-bretagne.fr/redmine/projects/show/geobretagne2 pour avoir accès à 
l'ensemble des informations

Technical
==========

What are the standards implemented in geOrchestra ?
---------------------------------------------------

geOrchestra uses the OGS standards, including :

* `WMS <http://www.opengeospatial.org/standards/wms>`_ : Web Map Service
* `WMTS <http://www.opengeospatial.org/standards/wmts>`_ : Web Map Tile Service
* `WFS <http://www.opengeospatial.org/standards/wfs>`_ : Web Feature Service
* `WCS <http://www.opengeospatial.org/standards/wcs>`_ : Web Coverage Service
* `WMC <http://www.opengeospatial.org/standards/wmc>`_ : Web Map Context
* `SLD <http://www.opengeospatial.org/standards/sld>`_ : Styled Layer Descriptor
* `FE <http://www.opengeospatial.org/standards/filter>`_ : Filter Encoding
* `CSW <http://www.opengeospatial.org/standards/cat>`_ : Catalog Service
* `WPS <http://www.opengeospatial.org/standards/wps>`_ : Web Processing Service

What is the limit of 114 KB which sometimes appears in MapFishApp ?
-------------------------------------------------------------------

This is a limitation in the MapFishApp javascript code to avoid treatments potentially too heavy in the client. 
We voluntarily limit the size of XML streams acceptable, and this limit is scalable depending on the browser. 
Example: IE 6 => limited ability to parse XML => lower limit.


There are three reasons why this happens:

* all EPSG codes are listed in GetCapabilities;
* all the layers are in the same namespace or you do not use namespace in the services URL (eg http://myserver/geoserver/wms);
* you have too many layers in the namespace (same reason as the previous point).

In the end it leads to a too large size for the GetCapabilities XML file.

To correct this problem :

* list the EPSG codes that must be available in GeoServer ;
* place the layers in different namespaces ;
* use the url with namespace: http://myserver/geoserver/myNamespace/wms.


Address search does not work ...
--------------------------------

You must install the module :ref:`georchestra.en.documentation.search_address`.


How to connect research repositories ?
--------------------------------------

See :ref:`georchestra.en.documentation.postinstall`.


In edit mode, the page slowed sharply, I have an error message
--------------------------------------------------------------

JavaScript performance is highly dependent on the web browser used and IE shall not be deemed to have excellent performance in this. 
Generally you have this problem in the editor when you want to edit a layer having a high amount of vertices/points.

There is no solution.


How to extend the format types available in the extractorapp ?
--------------------------------------------------------------

It's not possible at this moment.
You can finance this development.


Unable to add a raster data (ecw, jpg2000 ...)
----------------------------------------------

You must install additionnals plugins in Geoserver.
You can see the `geomatips blog <http://geomatips.blogspot.com/2010/02/support-de-lecw-dans-geoserver.html>`_ 
or `Geoserver documentation <http://docs.geoserver.org/>`_.
