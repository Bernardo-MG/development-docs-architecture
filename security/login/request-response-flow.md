# Request-Response Flow

<figure><img src="../../.gitbook/assets/login_request_flow.drawio.png" alt=""><figcaption><p>Login request flow</p></figcaption></figure>

1. User fills form
2. Login request is sent to the backend
   * Request is validated
   * Login status is returned to the frontend
3. Frontend handles status response
   * If successful, the user is now authenticated
   * Otherwise, the user isn't authenticated



The frontend sends a request for a login attempt. Receiving the response with the status of said login attempt. If successful the status will contain any additional detail as required, such as auth tokens.

All calculations or operations are handled by the backend.
