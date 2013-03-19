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







