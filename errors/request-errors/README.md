# Request Errors

<figure><img src="../../.gitbook/assets/flow_request_error.drawio.png" alt=""><figcaption></figcaption></figure>

This is oriented to a frontend-backend communication, so only those errors which occur when the backend processes a request matter here. The errors will be split between the frontend and backend, depending on who can handle them.

* Failures are those errors which the frontend can fix.
* Internal errors are those errors detected in the backend which the frontend can't fix.
