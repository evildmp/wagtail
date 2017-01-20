Deploying Wagtail
-----------------

On your server
~~~~~~~~~~~~~~

Wagtail is straightforward to deploy on modern Linux-based distributions, but see the section on :doc:`performance </advanced_topics/performance>` for the non-Python services we recommend.

Our current preferences are for Nginx, Gunicorn and supervisor on Debian, but Wagtail should run with any of the combinations detailed in Django's `deployment documentation <https://docs.djangoproject.com/en/dev/howto/deployment/>`_.

On Gondor
~~~~~~~~~

`Gondor <https://gondor.io/>`_ specialise in Python hosting. They provide Redis and Elasticsearch, which are two of the services we recommend for high-performance production sites. Gondor have written a comprehensive tutorial on running your Wagtail site on their platform, at `gondor.io/blog/2014/02/14/how-run-wagtail-cms-gondor/ <https://gondor.io/blog/2014/02/14/how-run-wagtail-cms-gondor/>`_.

On Openshift
~~~~~~~~~~~~

`OpenShift <https://www.openshift.com/>`_ is Red Hat's Platform-as-a-Service (PaaS) that allows developers to quickly develop, host, and scale applications in a cloud environment. With their Python, PostgreSQL and Elasticsearch cartridges there's all you need to host a Wagtail site. To get quickly up and running you may use the `wagtail-openshift-quickstart <https://github.com/texperience/wagtail-openshift-quickstart>`_.

On Divio Cloud
~~~~~~~~~~~~~~

The `Divio Cloud <https://divio.com>`_ provides dedicated Django hosting. It's an application-centric platform, and
includes Wagtail amongst its base project types, so you can have a live Wagtil project running in minutes. Projects on
Divio Cloud run in Docker containers, which can be also be built locally to provide you with a development environment
that's identical to the deployment environment. See `Get started with Wagtail
<http://support.divio.com/project-types/wagtail/get-started-with-wagtail-on-divio-cloud>`_ in the Divio Cloud
documentation, and `Deploy your Wagtail site on Divio <add-link-to-Wagtail-weblog>`_ in the Wagtail weblog.

On other PAASs and IAASs
~~~~~~~~~~~~~~~~~~~~~~~~

We know of Wagtail sites running on `Heroku <http://spapas.github.io/2014/02/13/wagtail-tutorial/>`_, Digital Ocean and elsewhere. If you have successfully installed Wagtail on your platform or infrastructure, please :doc:`contribute </contributing/index>` your notes to this documentation!
