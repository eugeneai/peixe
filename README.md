The Aquarium Project
====================

(The web page is at http://eugeneai.github.com/aquarium/)

Already so tired of filling in various document papers... Why not fill the in a forms and just print and sign. Or... save their field content in a database or QR-code? Later the data can be used again.

Sometimes in a preparation of a draft treaty texts small error must be corrected in all its descendants simultaneously.

In this project we will try do develop an engine to support inductive interactive processing of textual documents:
 * Compare set of *almost* identical documents and induce (not deduce) forms to be filled in;
 * so, self-educated [Auto]Filling engine (AFE);
 * Domain ontology induction as thesauruses and using it in the AFE;
 * Document structure induction and arrange it in an ontology also;
 * Document structure user interface and AFE support;
 * etc.

Later we will try to "mine" a relational database structures from the data collected.

"Do not feed a programmer, allow him/her to share his/her plans for the future" (c) Smbdy from Novosibirsk programming school of 1980-ths.

Evgeny

Shortcut links:
 * [List of potetially useful IT](https://github.com/eugeneai/aquarium/blob/master/collection/LIBS.md)


Temporal documentation chunks
-----------------------------

Before the installation a python-2.7 virtual evnironment should be set
up in the apckage directory, e.g.

    virtualenv-2.7 python2

and, optionally, run

    . python2/bin/activate


To setup run in the virtual environment

    python2/bin/python2 setup.py develop

and run it with pserve:

    python2/bin/pserve deployment.ini

To run uWSGI instance in ubuntu

    uwsgi_python --ini-paste deployment.ini

the same in Arch Linux (Does not work now. It says, that the socket is
not defined.)

    uwsgi_python2 --ini-paste deployment.ini

and point your browser (now the application is a stub, it does nothing):

    http://<server name or ip or 127.0.0.1>:6543/

e.g.

    http://127.0.0.1:6543/

But it is not useful now. Sorry.
