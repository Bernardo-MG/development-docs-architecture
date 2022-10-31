# Pagination Observer

An URL observers allows reacting to changes on the URL pagination parameters.

<figure><img src="../../../.gitbook/assets/pagination_observer_frontend_class.drawio (2).png" alt=""><figcaption><p>Pagination Observer</p></figcaption></figure>

## Use

* Give the pagination data when it changes on the URL

## Flow

When those parameters change:

* A new pagination object is prepared
* A new request is made with the pagination
* The response of the request contains the current pagination status

## Data

* Full pagination data
