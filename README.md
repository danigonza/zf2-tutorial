zf2-tutorial
============

Zend Framework 2 Akrabat Tutorial

Install zf2 skeleton app
------------------------

### Download composer ###

<pre><code>curl -s https://getcomposer.org/installer | php</code></pre>

### Download ZF2 Application Skeleton ###

<pre><code>php composer.phar create-project --repository-url="http://packages.zendframework.com" zendframework/skeleton-application path/to/install</code></pre>

### VirtualHost ###

<pre><code>
&lt;VirtualHost *:80&gt; 
    ServerName zf2-tutorial.localhost 
    DocumentRoot /path/to/zf2-tutorial/public 
    SetEnv APPLICATION_ENV &quot;development&quot; 
    &lt;Directory /path/to/zf2-tutorial/public&gt; 
      DirectoryIndex index.php 
      AllowOverride All 
      Order allow,deny 
      Allow from all 
    &lt;/Directory&gt; 
&lt;/VirtualHost&gt;
</code></pre>

**Wait!** Make sure that you zf2-tutorial.localhost is mapped to 127.0.0.1

Tutorial
--------

You can follow this tutorial here: http://zf2.readthedocs.org/en/latest/user-guide/overview.html

Album Module
------------

1.   Create the Module class for the Album module
2.   Create the autoload_classmap file
3.   Create the module.config file
4.   Update the application config file

Routing and controllers
-----------------------

1.  Add the routes for the specific controller & actions
2.  Create the controller

Database and models
-------------------

1.  Create the database and the tables
2.  Create the entity models
3.  Crete the TableGateway classes
4.  Configure Service Manager
5.  Configure the connection with the db (global parameters and local parameters)

Styling and Translations
------------------------

1.  Add lang strings
2.  Modify app layout

Forms and actions
-----------------

1.  Create forms
2.  Add the filter and validators to the entity model
3.  Call form from controllerer's actions
4.  Render forms in views
5.  Force to show list in app index







