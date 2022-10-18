# Request-Response

## Request

<figure><img src="../../.gitbook/assets/login_request_flow.drawio.png" alt=""><figcaption><p>Login request flow</p></figcaption></figure>

The frontend sends a request for a login attempt. Receiving the response with the details of said login attempt. These details tell the status of the attempt and, if it was successful, contain any additional detail, such as auth tokens.

All calculations or operations are handled by the backend.

## Model

<figure><img src="../../.gitbook/assets/login_model.drawio.png" alt=""><figcaption></figcaption></figure>

The LoginRequest is used on the request.

LoginDetails is the response returned after the login attempt. If the attempt failed then the logged flag is set as false.

## Flow

