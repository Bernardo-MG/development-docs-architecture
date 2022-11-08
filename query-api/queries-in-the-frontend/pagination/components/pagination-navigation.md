# Pagination Navigation

The navigation component should be able to change the route, and update itself when it changes. For this reason it requires and actuator and observer.

![Pagination navigation](../../../../.gitbook/assets/pagination\_navigation\_frontend\_class.drawio.png)

## Use

* Change the current page
* Update when the page is changed

## Route Flow

When the user navigates to another page:

* The actuator updates the route parameters

When the URL pagination parameters change:

* The navigation updates the data shown

## Data

* Current page
* First/last page flag

## How it works

The previous and next buttons depend on the first and last page flag. As long as it is not the first page, it allows going back to the previous one. The same for the next page if it isn't the last one.

The current page is shown in a text input, which can be edited to change to another page.

All these cases end in the same
