zf2-tutorial
============

[![Build Status](https://travis-ci.org/danigonza86/zf2-tutorial.png)](https://travis-ci.org/danigonza86/zf2-tutorial)

Zend Framework 2 Akrabat Tutorial

Install zf2 skeleton app [Git Tag: zf-tutorial](https://github.com/danigonza86/zf2-tutorial/tree/zf2-tutorial)
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

Testing with phpunit [Git Tag: zf-tutorial-phpunit](https://github.com/danigonza86/zf2-tutorial/tree/zf2-tutorial-phpunit)
--------------------

Follow the steps in this tutorial: http://zf2.readthedocs.org/en/latest/tutorials/unittesting.html

1.  Setting up the tests directory
2.  Bootstrapping your tests
3.  Your first Controller test
4.  A failing test case
5.  Configuring the service manager for the tests
6.  Testing actions with POST
7.  Testing model entities
8.  Testing model tables

Working with Doctrine2 [Git Tag: zf-tutorial-Doctrine2](https://github.com/danigonza86/zf2-tutorial/tree/zf2-tutorial-Doctrine2)
----------------------

To work with doctrine2 in this tutorial I followeed this:

*   Jason Grimes tutorial: http://www.jasongrimes.org/2012/01/using-doctrine-2-in-zend-framework-2/
*   Marco Pivetta slides: http://marco-pivetta.com/doctrine-orm-zf2-tutorial/
*   To verify, this bitbucket repo: https://bitbucket.org/anjheu/zf2_doctrine2

1.  Install Doctrine modules
2.  Create the Album entity  
3.  Update the Album controller to use Doctrine instead of Zend_Db  
4.  Install zendframework-developer-tools 


Adding Navigation [Branch navigation](https://github.com/danigonza86/zf2-tutorial/tree/navigation)
----------------------

Follow this tutorial: http://zf2.readthedocs.org/en/latest/tutorials/tutorial.navigation.html

1.  Preparation
2.  Setting Up Zend\Navigation
3.  Configuring our Site Map
4.  Adding the Menu View Helper
5.  Adding Breadcrumbs

