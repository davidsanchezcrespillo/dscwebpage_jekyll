---
layout: default
title: "CV"
---

<p><a href="#publications">Publications</a> | <a href="#master-thesis">Master Thesis</a></p>

# CV

Find below a __100-words version__ of my CV. For more details, check my [LinkedIn profile](https://www.linkedin.com/in/davidsanchezcrespillo).

### Work experience

  * [European Commission](https://ec.europa.eu). Information and Communication Assistant. __2012 - present__.
  * [Acapela Group](http://www.acapela-group.com) (Voice Software - Belgium). Software Engineer. __2010-2012__.
  * [Government of the Balearic Islands](http://www.caib.es) (Government - Spain). ICT Teacher. __2006-2010__
  * [Gridsystems](http://www.gridsystems.com) (Grid Software - Spain). Software Engineer. __2000-2006__
  * [University of Balearic Islands](http://www.uib.es) (University - Spain). 3D Programmer and Researcher. __1998-2000__
  * [Infomallorca IAE](http://www.infomallorca.net) (Touristic Services - Spain). Computer Operator. __1997-1998__

### Education

  * [University of Balearic Islands](http://www.uib.es). Engineer in Computer Science.  __2000__
  * [University of Balearic Islands](http://www.uib.es). Official Teaching Certificate. __2003__

### Languages

  * __Spanish__ (Native), __Catalan__ (Native), __English__ (C2), __French__ (B2).

### Skills

  * Development (Java, PHP, Perl, C++, C#).
  * Tools (Unit Testing, Continuous Integration, Version Control).
  * Responsible, methodical, proactive, pragmatic, curious.

---

## Publications

Some publications in which I participated as part of my job in the [University of the Balearic Islands](http://www.uib.es), and also much later as a 
teacher.

<div>
{% include render_publications.html %}
</div>

---

## Master Thesis

My [Master Thesis]({{ '/media/pdf/proyecto_000920.pdf' | prepend:site.baseurl }}) for the Degree of __Engineer in Computer Science__, in the [University of the Balearic Islands](http://www.uib.es), was defended the 20th of October 2000, and __awarded with honors__.

The title of the thesis was __Desarrollo de técnicas cooperativas para un editor de objetos 3D__ (Development of cooperative techniques for a 3D editor) and was directed by the professors Ricardo Galli Granada and Yuhua Luo.

![PDF Icon]({{ '/media/img/pdf.png' | prepend:site.baseurl }} "PDF Icon") [Desarrollo de técnicas cooperativas para un editor de objetos 3D]({{ '/media/pdf/proyecto_000920.pdf' | prepend:site.baseurl }}) (in Spanish)

### Abstract

Development of cooperative techniques for the editing of 3D objects, by applying and extending the Mu3D high level protocol. These techniques are applied to the basic operations of an architecture-oriented 3D editor. The operations include: Concurrency control, data management, basic editing (object insertion and deletion, interactive geometric transformation, material editing and lightning parameters), clipboard operations and undo.

The system implements a completely distributed architecture, and uses JESP, a cooperative work support platform, which deals with the session and group communication management. On this platform, the M3D Editor, an interactive architecture-oriented 3D editor, is executed.

The special features of the 3D data (high amount of data, need of fast interactive visualization) require to provide local access to the data. Due to this, data are replicated on each workstation, following a paradigm called distributed shared memory with active replication.

Data replication makes necessary keeping its consistency on all the replicas. Every modification on the replicated data has to be notified to the rest of users. On the other hand, notification messages should be as small as possible, to allow updates at interactive speed.

The concurrent access control is implemented using an implicit locking system, based on selections of the 3D objects.

