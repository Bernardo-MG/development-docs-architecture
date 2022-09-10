# Pagination Observer



<figure><img src="../../../../.gitbook/assets/angular_observer.drawio (1).png" alt=""><figcaption></figcaption></figure>

The RoutePaginationObserver watches for changes in pagination.

* Listens for changes in the route parameters
  * Only reacts for pagination parameters
  * If one changes, throws an event
* Will watch the current route
* To use, just listen to its page change event
* Can be used in any component, as needed
