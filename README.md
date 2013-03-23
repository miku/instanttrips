README
======

Instanttrips is an instant-ish interface to an elasticsearch based
SPO (subject-predicate-object) index. An SPO index can be seen
as a *very* stripped down triple-store. In fact, the documents that get
pushed to the index looks just like this:

	{
		"s": "http://dbpedia.org/resource/Arild",
		"p": "http://xmlns.com/foaf/0.1/homepage",
		"o": "http://www.arildsbyalag.nu"
	}

Screenshots
-----------

[http://imgur.com/a/jxnSZ](http://imgur.com/a/jxnSZ)


Remarks
-------

As long as the data does not contain to many blank nodes, this prototype
is ok, because you can find your data within seconds (with datasets in the 
order of millions of triples). With blank nodes, the tabular structure
breaks down.

More on blank nodes:

> I haven't gotten to the problem yet. As Pat Hayes points out, the problem is most clearly exposed by blank nodes. Blank nodes are parts of a knowledge representation that don't have global identity; they're put in as a kind of glue that connects parts of a fact.
([http://go-to-hellman.blogspot.de/2009/11/blank-node-bother-and-rdf-copymess.html](http://go-to-hellman.blogspot.de/2009/11/blank-node-bother-and-rdf-copymess.html.))

* [Problems of the RDF model: Blank nodes](http://milicicvuk.com/blog/2011/07/14/problems-of-the-rdf-model-blank-nodes/)

* [An Alternative to the Top-Down Semantic Web of Services](http://www-cdr.stanford.edu/~petrie/online/peer2peer/semanticscripts.pdf)