# Storing Queries in the Route

We want to use the route to store any data which may define the view, such as the current page. This way reusing a URL will arrive at the same view, with the same context.

## Usage Example

We have the URL https://somewhere.com/employees?page=2. This loads the third page (they start with the index 0). The user wants to store this URL, so he always returns to the same page. Of course, this doesn't mean the page will always show the same data, but it will show the same context.

This extends to several cases:

* Pagination (page number, page size)
* Ordering (fields, direction)
* Filtering (field, comparison, value)

## Limits

There is a single route for each view, so the context is applied to the full page. For example, this would support a single paginated set.

## Generic Design

<figure><img src="../../../../.gitbook/assets/general_flow.drawio.png" alt=""><figcaption><p>URL flow</p></figcaption></figure>

Reading and writing parameter are two distinct flows. They are kept isolated, so the only way they can interact is through the URL.

The controller works as a mediator, keeping all the code required for these operations.

## Example

As shown in the diagram, we will use pagination as an example.

* When changing the page, the current page number is set into the route parameters.
* When showing the current page, the page parameter is read from the route parameters and returned to the view.

Measures should be taken to avoid ending in a circular flow, which reads and writes parameters in a loop.
