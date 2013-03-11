Atom-PMH
========

Introduction
------------

The _Atom Feed Protocol for Metadata Harvesting_ (Atom-PMH) is a
protocol for harvesting metadata.

It performs a similar function to [OAI-PMH], except it uses Atom 1.0 and
is a RESTful protocol. This gives it performance and implementation
advantages over OAI-PMH.

This project contains the specification for Atom-PMH.

[OAI-PMH]: <http://www.openarchives.org/pmh/>

Background
----------

The Atom-RDC specification was developed as part of an ANDS _Seeding
the Commons_ project and implemented in the UQ DataSpace system. In
DataSpace, AtomPub was used by research databases to publish
_metadata records_ into DataSpace.

That approach is not suitable for the _UQ Data Collections Registry_
going forward.  The use of AtomPub makes DataSpace the single
centralised source of truth. It makes it extremely difficult to
migrate from DataSpace. It also makes it extremely difficult for the
research databases to provide _metadata records_ to multiple systems
using the same approach. It takes the source of truth status away from
the research databases.

Therefore, there is a need to discontinue the use of AtomPub, but
provide a method of migration for those research databases that have
already implemented Atom-RDC. Requiring those research databases to
completely change to a different format (e.g. to RIF-CS) and a
different protocol (e.g. to OAI-PMH) is not practical in the short
term. The obvious solution, which has merits in its own right, is to
replace AtomPub with Atom 1.0 feeds.

Note: it is important to recognise that Atom 1.0, Atom-RDC and AtomPub
are designed for very different purposes and perform very different
functions. Despite the similar names they are very different
mechanisms.

Instructions
------------

The specification is written in [Markdown] (see files under the _posts
subdirectory) and is converted to HTML using [Jekyll]. The main (and
only) GitHub branch is "gh-pages" because the specification is automatically
published as the project's GitHub project pages.

To update the specification, create a new file under `_posts`
containing the new version. Do not modify the existing posts. Push the
changes to GitHub and (after a short delay) it will automatically
update the project pages at <http://uq-eresearch-spec.github.com/atom-pmh>.

[Markdown]: <http://daringfireball.net/projects/markdown/>

[Jekyll]: <https://github.com/mojombo/jekyll>

Contact
-------

For more information, please contact [Hoylen Sue](mailto:hoylen@hoylen.com)
or [The University of Queensland eResearch Lab](http://www.itee.uq.edu.au/eresearch/).

Acknowledgements
----------------

This project is supported by the Australian National Data Service
([ANDS](http://www.ands.org.au/)). ANDS is supported by the Australian
Government through the National Collaborative Research Infrastructure
Strategy Program and the Education Investment Fund (EIF) Super Science
Initiative.
