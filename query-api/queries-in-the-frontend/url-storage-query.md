# URL Query Storage

We want to define the current query inside the URL. Allowing the reuse of URLs to arrive always at the same view. Of course, this doesn't meant that the view will always show the same data, we are talking about about, for example, having a URL to arrive at the second page.

Useful for:

* Storing data we want to keep between visits

Which data can be stored in the URL?

* Page (page number, page size)
* Sort (fields, direction)
* Query (field, comparison, value)

## Flow

This works with two distinct flows. One for updating and another for reading. While both are handled by the controller, and both are bound to interactions in the view, they are to be kept isolated. The only way they can interact is through the URL.

<figure><img src="../../.gitbook/assets/general_flow.drawio.png" alt=""><figcaption></figcaption></figure>

Using pagination as the example. When a user request a page this changes the URL. Then the controller reacts to this change, reads the page and updated the data.
