{% if False %}
# Django 1.4 Base Template #

## About ##

This template is based off of the work of [Mozilla Playdoh][playdoh], as well as
experience with other Django layouts/templates. Playdoh is mainly setup for
Mozilla's systems, and is currently only designed for Django 1.3. Some of the
libraries bundled with Playdoh are also no longer necessary in Django 1.4.

This template is designed for Django 1.4's new startproject template option.

As much as I could, all the code has been updated to use the new suggested layout
and functionality in Django 1.4.

[playdoh]: https://github.com/mozilla/playdoh

## Features ##

By default, this template includes:

A set of basic templates built from HTML5Boilerplate 3.0.3 and Twitter Bootstrap 2.0 (located in the
base app)

Templating:

- Markdown

Security:

- bleach
- python-bcrypt2 - uses bcrypt for password hashing by default

Migrations:

- South

Caching:

- python-memcached

From Mozilla Playdoh:

- commonware
- nuggets

Admin:

- Includes django-admin-toolbar for development and production (enabled for superusers)
- Includes two debug-toolbar panels that are useful, but are disabled until they support Django 1.4
 - django-debug-toolbar-user-panel
 - memcache-debug-panel

Testing:

- nose and django-nose
- pylint, pep8, and coverage

Any of these options can added, modified, or removed as you like after creating your project.

## How to use this template to create your project ##

- Create your virtualenv
- Install Django 1.4
- $ django-admin.py startproject --template https://github.com/blorenz/django-base-template/zipball/master --extension py,md projectname
- $ cd projectname
- Select your database adapter in requirements/compiled.txt (MySQL, Postgresql, or stick with SQLite)
- $ pip install -r requirements/dev.txt
- $ cp projectname/settings/local-dist.py projectname/settings/local.py (local.py shouldn't be added
  to your source control)
- $ ./manage.py syncdb
- $ ./manage.py runserver

{% endif %}
# {{ project_name|title }} Project #

## About ##

Describe your project here.

## Prerequisites ##

- Python >= 2.5
- pip
- virtualenv (virtualenvwrapper is recommended for use during development)

## Installation ##

Fill out with installation instructions for your project.


License
-------
This software is licensed under the [New BSD License][BSD]. For more
information, read the file ``LICENSE``.

[BSD]: http://opensource.org/licenses/BSD-3-Clause
