# Request-Response Model

<figure><img src="../../.gitbook/assets/login_model.drawio.png" alt=""><figcaption><p>Login model</p></figcaption></figure>

The LoginRequest is, as it says, the request for a log in attempt.

LoginStatus is the response after that login attempt. Mainly it tells of the attempt was successful or not, through the logged flag. But it may contain additional info, such as authentication tokens.

