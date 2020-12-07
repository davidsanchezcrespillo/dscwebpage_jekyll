---
layout: default
title: "Publications"
---

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
