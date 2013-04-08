.. _`georchestra.en.documentation.rfc`:

====================
RFC managment
====================

This section describes the operation of the RFC (Request For Comment). 
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

RFC vote
===============
The PSC is responsible for the RFC vote proposed by the community.
The process of voting is the following one:

* each PSC member has one vote which can be -1 (rejection), -0, +0, +1 
  (acceptance) ;
* a PSC member who vote negatively must provode a minimum of explanation ;
* a PSC member who vote negatively has to propose an alternative solution in a limited time ;
* a vote "-0" indicates soft disagreement, but has no effect. The vote "0" indicates no opinion. 
  A vote "+0" indicates a soft support, but has no effect ;
* the RFC author must argue back a minimum for its proposal ;
* a negative vote is analyzed to see how to change the blocking criterion in order to have a positive vote ;
* the proposal is considered accepted after an absolute majority  for vote "+1" and all comments 
  for the negative votes have been resolved.
  The author of the proposal has to announce if this one is accepted (proposal accepted by the majority of committers) 
  or if he removes its proposal (veto). 

The president has a vote. It is responsible for maintaining an updated list of
PSC members of the project. Adding and removing a PSC member, as well as the selection of a president 
should be treated as a proposal to the PSC.

The president rules in the cases of disputes on a vote.

A proposal will be accepted only if it receives +2 (author included) and no veto (-1).

If a veto is opposed to a proposal, and if this proposal can't be reviewed to satisfy all voters,
then the proposal may be submitted for another vote in which a majority of all eligible voters
indicating "+1" is sufficient to adopt it.
Note that it is the majority of all the PSC members, and not only those who effectively voted.


Implementing a RFC
===========================

The proposed, discussed and voted RFC are available in the github project 
`geOrchestra (pull request) <https://github.com/georchestra/georchestra>`_ .

When voting is mandatory ?
====================================

The vote is mandatory in the following cases :

* Any change in the PSC composition (new members or deleting inactive members)
* Changes to the infrastructure project (eg tool, location, main configuration)
* Anything that can cause problems with backward compatibility.
* Adding large contributions of new code.
* Inter-subsystem API or objects changes.
* Procedural matters.
* In case of release.
* While relations with external entities such as OSGeo.
* Anything that might be controversial.



