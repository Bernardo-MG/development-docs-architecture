# Design

![Flows handled through components](../../../.gitbook/assets/datasource\_url\_flow.drawio.png)

We will use a component for each flow, with no dependency between them:

* The actuator reacts to an order to update the route parameters
* The observer watches the route and reacts to changes

## Observer: Reading parameters

Whenever the URL parameters change. In practice, this means when loading a URL.

1. URL argument is read (page number)
2. Data is read (read for page)

## Actuator: Writing parameters

Done by the user. When using an UI component.

1. User makes use of an actuator (next page)
2. URL is updated (set page number)
3. New URL argument is read (page number)
4. Data is updated (read for page)

## Cases

### Loading a view for the first time

1. Route: /employees
2. Read route arguments
   1. No arguments
3. Request with no arguments (initial request)
   1. Loads initial values from the request
4. Final route: /employees

### Changing page

1. Route: /employees
2. Update page argument
   1. Read current page (page 0)
   2. Increase page value (page 1)
   3. Set page argument
3. Move to route: /employees?page=1
4. Reload view
5. Final route: /employees?page=1

### Load a view with arguments

1. Route: /employees?page=1
2. Read route arguments
   1. Page 1
3. Request using these arguments
4. Final route: /employees?page=1
