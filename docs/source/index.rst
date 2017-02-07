.. _topics-index:

================================
Frontera |version| 文档
================================

`Frontera`_ is a web crawling tool box, allowing to build crawlers of any scale and purpose.
`Frontera`_ 是一个爬虫工具箱，它可以让你构建任何规模和目的的爬虫。

`Frontera`_ provides :ref:`crawl frontier <crawl-frontier>` framework by managing *when* and *what* to crawl next,
and checking for *crawling goal* accomplishment.
`Frontera`_ 提供 :ref:`crawl frontier <crawl-frontier>` 框架，这个框架可以帮助管理*何时抓取下一个URL*、*下个抓取的URL是什么*和检查*抓取结果*

Frontera also provides replication, sharding and isolation of all crawler components to scale and distribute it.

Frontera contain components to allow creation of fully-operational web crawler with `Scrapy`_. Even though it was
originally designed for Scrapy, it can also be used with any other crawling framework/system as the framework offers
a generic tool box.


Introduction
============

The purpose of this chapter is to introduce you to the concepts behind Frontera so that you can get an idea of
how it works and decide if it is suited to your needs.

.. toctree::
   :hidden:

   topics/overview
   topics/run-modes
   topics/quick-start-single
   topics/quick-start-distributed
   topics/cluster-setup

:doc:`topics/overview`
    Understand what Frontera is and how it can help you.

:doc:`topics/run-modes`
    High level architecture and Frontera run modes.

:doc:`topics/quick-start-single`
    using Scrapy as a container for running Frontera.

:doc:`topics/quick-start-distributed`
    with SQLite and ZeroMQ.

:doc:`topics/cluster-setup`
    Setting up clustered version of Frontera on multiple machines with HBase and Kafka.

Using Frontera
==============

.. toctree::
   :hidden:

   topics/installation
   topics/frontier-objects
   topics/frontier-middlewares
   topics/frontier-canonicalsolvers
   topics/frontier-backends
   topics/message_bus
   topics/own_crawling_strategy
   topics/scrapy-integration
   topics/frontera-settings

:doc:`topics/installation`
    HOWTO and Dependencies options.

:doc:`topics/frontier-objects`
    Understand the classes used to represent requests and responses.

:doc:`topics/frontier-middlewares`
    Filter or alter information for links and documents.

:doc:`topics/frontier-canonicalsolvers`
    Identify and make use of canonical url of document.

:doc:`topics/frontier-backends`
    Define your own crawling policy and custom storage.

:doc:`topics/message_bus`
    Built-in message bus reference.

:doc:`topics/own_crawling_strategy`
    Implementing own crawling strategy for distributed backend.

:doc:`topics/scrapy-integration`
    Learn how to use Frontera with Scrapy.

:doc:`topics/frontera-settings`
    Settings reference.


Advanced usage
==============

.. toctree::
   :hidden:

   topics/what-is-cf
   topics/graph-manager
   topics/scrapy-recorder
   topics/fine-tuning
   topics/dns-service

:doc:`topics/what-is-cf`
    Learn Crawl Frontier theory.

:doc:`topics/graph-manager`
    Define fake crawlings for websites to test your frontier.

:doc:`topics/scrapy-recorder`
    Create Scrapy crawl recordings and reproduce them later.

:doc:`topics/fine-tuning`
    Cluster deployment and fine tuning information.

:doc:`topics/dns-service`
    Few words about DNS service setup.

Developer documentation
=======================

.. toctree::
   :hidden:

   topics/architecture
   topics/frontier-api
   topics/requests-integration
   topics/examples
   topics/tests
   topics/loggers
   topics/frontier-tester
   topics/faq
   topics/contributing
   topics/glossary




:doc:`topics/architecture`
    See how Frontera works and its different components.

:doc:`topics/frontier-api`
    Learn how to use the frontier.

:doc:`topics/requests-integration`
    Learn how to use Frontera with Requests.

:doc:`topics/examples`
    Some example projects and scripts using Frontera.

:doc:`topics/tests`
    How to run and write Frontera tests.

:doc:`topics/loggers`
    A list of loggers for use with python native logging system.

:doc:`topics/frontier-tester`
    Test your frontier in an easy way.

:doc:`topics/faq`
    Frequently asked questions.

:doc:`topics/contributing`
    HOWTO contribute.


:doc:`topics/glossary`
    Glossary of terms.



.. _Crawling System: http://en.wikipedia.org/wiki/Web_crawler
.. _Scrapy: http://scrapy.org/
.. _`Frontera`: http://github.com/scrapinghub/frontera