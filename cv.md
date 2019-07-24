---
layout: default
title: "CV"
---

## In 100 words

[LinkedIn profile](https://www.linkedin.com/in/davidsanchezcrespillo)

__Work experience__

  * __2012-now__. [European Commission](https://ec.europa.eu). Information and Communication Assistant.
  * __2010-2012__. [Acapela Group](https://www.acapela-group.com) (Voice Software - Belgium). Software Engineer. 
  * __2006-2010__. [Government of the Balearic Islands](http://www.caib.es) (Government - Spain). ICT Teacher. 
  * __2000-2006__. __Gridsystems__ (HPC Software - Spain). Software Engineer. 
  * __1998-2000__. [University of Balearic Islands](http://www.uib.es) (University - Spain). 3D Programmer and Researcher.
  * __1997-1998__. __Infomallorca IAE__ (Touristic Services - Spain). Computer Operator. 

__Education__

  * [University of Balearic Islands](http://www.uib.es). Engineer in Computer Science.  __2000__
  * [University of Balearic Islands](http://www.uib.es). Official Teaching Certificate. __2003__

__Skills__

  * Development (Java, PHP, Perl, C++, C#).
  * Tools (Unit Testing, Continuous Integration, Version Control).
  * Responsible, methodical, proactive, pragmatic, curious.

Languages: __Spanish__ (Native), __Catalan__ (Native), __English__ (C2), __French__ (B2).

__Publications__

<div>
{% include render_publications.html %}
</div>

__Master Thesis__

![PDF Icon]({{ '/media/img/pdf.png' | prepend:site.baseurl }} "PDF Icon") [Desarrollo de técnicas cooperativas para un editor de objetos 3D]({{ '/media/pdf/proyecto_000920.pdf' | prepend:site.baseurl }}) (in Spanish)

Thesis submitted in partial fulfillment of the requirements for the degree of __Engineer in Computer Science__, in the [University of the Balearic Islands](http://www.uib.es). Directed by the professors Ricardo Galli Granada and Yuhua Luo. Defended on 20 October 2000. Awarded with honors.

<div class="well">
<p><strong>Abstract: Development of cooperative techniques for a 3D editor.</strong>
</p>
<p>
Development of cooperative techniques for the editing of 3D objects, by applying and extending the Mu3D high level protocol. These techniques are applied to the basic operations of an architecture-oriented 3D editor. The operations include: Concurrency control, data management, basic editing (object insertion and deletion, interactive geometric transformation, material editing and lightning parameters), clipboard operations and undo.
</p>
<p>
The system implements a completely distributed architecture, and uses JESP, a cooperative work support platform, which deals with the session and group communication management. On this platform, the M3D Editor, an interactive architecture-oriented 3D editor, is executed.
</p>
<p>
The special features of the 3D data (high amount of data, need of fast interactive visualization) require to provide local access to the data. Due to this, data are replicated on each workstation, following a paradigm called distributed shared memory with active replication.
</p>
<p>
Data replication makes necessary keeping its consistency on all the replicas. Every modification on the replicated data has to be notified to the rest of users. On the other hand, notification messages should be as small as possible, to allow updates at interactive speed.
</p>
<p>
The concurrent access control is implemented using an implicit locking system, based on selections of the 3D objects.
</p>
</div>
