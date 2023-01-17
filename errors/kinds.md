# Request Errors

<figure><img src="../.gitbook/assets/flow_request_error.drawio.png" alt=""><figcaption></figcaption></figure>

This is oriented to a frontend-backend communication, so only those errors which occur when the backend processes a request matter here. The errors will be split between the frontend and backend, depending on who can handle them.

* Failures are those errors which the frontend can fix.
* Internal errors are those errors detected in the backend which the frontend can't fix.

## Failures

Invalid requests. Frontend errors which can be fixed by the user or the client.

### Validation failure

<figure><img src="../.gitbook/assets/validation_error_response_model.drawio.png" alt=""><figcaption></figcaption></figure>

## Internal Error

<figure><img src="../.gitbook/assets/generic_error_response_model.drawio.png" alt=""><figcaption></figcaption></figure>

Backend failures. Can't be fixed by the user or the client.

There are two additional kinds:

* Fixable errors. The frontend won't know this happened, the backend fixes them.
* Fatal errors. Which can't be fixed, these stop the process.
