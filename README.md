Sphene Community Tools (SCT) - http://sct.sphene.net
Copyright (C) by Herbert Poul (herbert.poul@gmail.com)


Sphene Community Tools are django applications to build communities and 
similiar websites designed to be easily pluggable into any django 
project to build.
It currently consists of a forum, wiki and blog application.


## Directories

- sphenecoll/	Collection of django application (the base source for SCT).
- examples/     A simple example configuration for using forum and wiki


## Requirements

- [Django](http://www.djangoproject.com) 2.0 or later
- Python >= 3.6
- [Python Imaging Library (Pillow)](https://pillow.readthedocs.io/)

## Installation

(Note: Since 0.6 SCT also comes with an experimental setup.py - if you
are using (e.g. by executing: python setup.py install) please provide
feedback on http://sct.sphene.net/ or herbert.poul@gmail.com if it 
worked or if you encountered any problems.)

To find instructions on how to setup a simple project for using forum
and wiki see our tutorial at:
http://sct.sphene.net/wiki/show/Tutorial/

### Python library path

You need to add sphenecoll/ to your python include path.

### Maintenance cron job (Optional)

To recaulcate heat for forum threads and similar, you should add the following
cronjob to run once a day (or similar)

    /path/to/your/django/project/manage.py sph_maintenance

### Cache

SCT makes use of django caching framework - it is therefore advised to 
configure CACHE_BACKEND django setting & co.
look at the [django caching documentation](http://www.djangoproject.com/documentation/cache/)

### Search

Please follow the [search documentation](http://sct.sphene.net/wiki/show/Search/).

## Examples

There are currently two examples - a very simplistic 'simpleproject' in the
examples/ directory (see examples/simpleproject/README) and a more
sophisticated example called CommunityDraft which i recommend as using as a base for your
own projects (if you start from scratch).
See <http://sct.sphene.net/wiki/show/CommunityDraft/> for details.


