# Request-Response

## Request

<figure><img src="../../.gitbook/assets/login_request_flow.drawio.png" alt=""><figcaption><p>Login request flow</p></figcaption></figure>

The frontend sends a request for a login attempt. Receiving the response with the status of said login attempt. If successful the status will contain any additional detail as required, such as auth tokens.

All calculations or operations are handled by the backend.

## Model

<figure><img src="../../.gitbook/assets/login_model.drawio.png" alt=""><figcaption><p>Login model</p></figcaption></figure>

The LoginRequest is, as it says, the request for a log in attempt.

LoginStatus is the response after that login attempt. Mainly it tells of the attempt was successful or not, through the logged flag. But it may contain additional info, such as authentication tokens.

