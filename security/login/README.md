# Login

Authenticates a user. The frontend offers a form, which takes the credentials and sends it to the backend.

## Flow

<figure><img src="../../.gitbook/assets/login_bpmn.drawio.png" alt=""><figcaption><p>Login request flow</p></figcaption></figure>

## Requests model



<figure><img src="../../.gitbook/assets/login_model.drawio.png" alt=""><figcaption><p>Login model</p></figcaption></figure>

The LoginRequest is, as it says, the request for a log in attempt.

LoginStatus is the response after that login attempt. Mainly it tells of the attempt was successful or not, through the logged flag. But it may contain additional info, such as authentication tokens.

The password is received, but never returned to the frontend.
