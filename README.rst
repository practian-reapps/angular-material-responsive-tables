########################################
angular-material-responsive-tables
########################################

.. class:: no-web

    Paquete para hacer responsivo a una ``table`` **html** usando css y angular



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

Example 2:

.. code-block:: html

                    <table table-responsive>
                        <caption>The Films of Hayao Miyazaki</caption>
                        <thead md-on-reorder="onReorder">
                            <tr>
                                <th rowspan='2'>#</th>
                                <th colspan='3'>Year dsadasd wwwww</th>
                                <th rowspan='2' class="col-hidden" data-search="Film" data-order="Film">Film</th>
                                <th rowspan='2'>Action</th>
                                <th colspan='2'>Ejem</th>
                                <th rowspan='2'>Honor</th>
                            </tr>
                            <tr>
                                <th>Year1</th>
                                <th>Year2</th>
                                <th>Year3</th>
                                <th class="col-hidden" data-search="Ejm1" data-order="Ejm1">Ejm1</th>
                                <th class="col-hidden" data-search="Ejm2" data-order="Ejm2">Ejm2</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>1</td>
                                <td>My Neighbor Totoro (Best Animated Feature)</td>
                                <td>1988</td>
                                <td>1988d</td>
                                <td>dsds</td>
                                <td>aa</td>
                                <td>eee1</td>
                                <td>ee2</td>
                                <td>Blue Ribbon Award ((Best Animated Feature))</td>
                            </tr>
                            <tr>
                                <td>1</td>
                                <td>Princess Mononoke</td>
                                <td>1997</td>
                                <td>1988d</td>
                                <td>dsds</td>
                                <td>aa</td>
                                <td>eee2</td>
                                <td>ee2</td>
                                <td>Nebula Award (Best Script)</td>
                            </tr>
                            <tr>
                                <td>1</td>
                                <td>Spirited Away</td>
                                <td>2001</td>
                                <td>1988d</td>
                                <td>dsds</td>
                                <td>aa</td>
                                <td>eee3</td>
                                <td>ee2</td>
                                <td>Academy Award (Best Animated Feature)</td>
                            </tr>
                            <tr>
                                <td>1</td>
                                <td>Howl’s Moving Castle</td>
                                <td>2004</td>
                                <td>1988d</td>
                                <td>dsds</td>
                                <td>aa</td>
                                <td>eee4</td>
                                <td>ee2</td>
                                <td>Hollywood Film Festival (Animation OTY)</td>
                            </tr>
                    </table>
Finally, run:

.. code-block:: bash

    #run
    $ gulp

Example:

.. code-block:: bash

    E:\practian-reapps\angular-material-responsive-tables>gulp
    [13:55:33] Using gulpfile E:\practian-reapps\angular-material-responsive-tables\gulpfile.js
    [13:55:33] Starting 'serve-browser-sync'...
    [13:55:33] Finished 'serve-browser-sync' after 449 ms
    [13:55:33] Starting 'watch'...
    [13:55:33] Finished 'watch' after 2.19 ms
    [13:55:33] Starting 'default'...
    [13:55:33] Finished 'default' after 6.71 μs
    [BS] Access URLs:
     -------------------------------
        Local: http://localhost:9103
     External: http://127.0.0.1:9103
     -------------------------------
    [BS] Serving files from: ./demo/




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







