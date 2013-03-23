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