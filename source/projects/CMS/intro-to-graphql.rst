Introduction to GraphQL
=======================

amFOSS CMS is based on GraphQL API. GraphQL is a query language which
offers much more flexibility for integrations. It allows you to request
the exact data you need, cutting down the number of calls you must
perform to get it. The availability of all data at one endpoint is also
the biggest advantage of GraphQL over the REST API (which has an
endpoint for each resource object).

There are two types of GraphQL APIs 1. Query 2. Mutation

Our API provides types of operations:

-  Public APIs
-  User APIs
-  Admin APIs

Click `here`_ to preview the API.

To learn more about GraphQL language and its concepts, see the official
GraphQL `website`_.

The endpoint remains constant regardless of the operation you perform.
Requests must be sent using the ``POST`` method and ``application/json``
content type.

.. _here: https://api.amfoss.in/
.. _website: https://graphql.org/
