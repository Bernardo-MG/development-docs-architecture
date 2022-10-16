# Storing Queries in the Route

We want to define the current query inside the URL route. Allowing the reuse of URLs to arrive always at the same view. Of course, this doesn't meant that the view will always show the same data, we are talking about about, for example, having a URL to arrive at the second page.

Useful for:

* Storing data we want to keep between visits

Which data can be stored in the URL?

* Page (page number, page size)
* Sort (fields, direction)
* Query (field, comparison, value)

## Problems

There is only a single route. This method can support a single paginated source per view.
