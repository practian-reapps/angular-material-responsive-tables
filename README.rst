########################################
angular-material-responsive-tables
########################################

.. class:: no-web

    Paquete para hacer responsivo a una ``table`` **htnml** usando css y angular



    .. image:: https://github.com/.. .png
        :alt: angular-material-responsive-tables
        :width: 100%
        :align: center



.. contents::

.. section-numbering::

.. raw:: pdf

   PageBreak oneColumn


============
Installation
============

-------------------
Dependencies
-------------------
- angular-material (not part of the bundle)
- angular-ui-router (not part of the bundle)
- angular (not part of the bundle)

-------------------
Development version
-------------------


The **latest development version** can be installed directly from github_:

.. code-block:: bash
    
    # Universal
    $ bower install https://github.com/practian-reapps/angular-material-responsive-tables.git --production --save


Add to your **index.html** setting like this:

.. code-block:: html

    <link rel="stylesheet" href="bower_components/angular-material-responsive-tables/dist/angular-material-responsive-tables.css" type="text/css" />
    
    <script src="bower_components/angular-material-responsive-tables/dist/angular-material-responsive-tables.js"></script>


Config module:

.. code-block:: js

    var app = angular.module("catalogo", [

    'pi.tableResponsive',

    'ui.router',
    'ngMaterial',
    'ngMdIcons',
]);

Usage:

.. code-block:: html

                        <table table-responsive>
                            <thead>
                                <tr>
                                    <th>#</th>
                                    <th>nombre</th>
                                    <th>direccion</th>
                                    <th>fecha_nac</th>
                                    <th>updated_at</th>
                                    <th colspan="2">acciones</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr ng-repeat="d in lista">
                                    <td> {{ (options.page - 1) * options.page_size +$index +1 }} </td>
                                    <td> {{ d.nombre }} </td>
                                    <td> {{ d.direccion }} </td>
                                    <td> {{ d.fecha_nac | date:'shortDate' }} </td>
                                    <td> {{ d.updated_at | date:'shortDate' }} </td>
                                    <td>
                                        u
                                    </td>
                                    <td>
                                        x
                                    </td>
                                </tr>
                            </tbody>
                        </table>


Finally, run ``gulp serve``.




====
Meta
====

-------
Authors
-------

- Angel Sullon Macalupu (asullom@gmail.com)



-------
Contributors
-------

See https://github.com/practian-reapps/angular-material-responsive-tables/graphs/contributors

.. _github: https://github.com/practian-reapps/angular-material-responsive-tables
.. _Django: https://www.djangoproject.com
.. _Django REST Framework: http://www.django-rest-framework.org
.. _Django OAuth Toolkit: https://django-oauth-toolkit.readthedocs.io
.. _oauth2_backend: https://github.com/practian-reapps/django-oauth2-backend
.. _Authorization server: https://github.com/practian-ioteca-project/oauth2_backend_service
.. _OAuth 2 Server Libraries: https://oauth.net/code
.. _Django backend utils: https://github.com/practian-reapps/django-backend-utils/blob/master/backend_utils/pagination.py







