# Pagination Navigation

The navigation component should be able to change the route, and update itself when it changes. For this reason it requires and actuator and observer.

![Pagination navigation](../../../../.gitbook/assets/pagination\_navigation\_frontend\_class.drawio.png)

## Use

* Change the current page
* Update when the page is changed

## Flow

When the user navigates to another page:

* The actuator updates the route parameters

When the URL pagination parameters change:

* The navigation updates the data shown

## Data

* Current page
* First/last page flag
