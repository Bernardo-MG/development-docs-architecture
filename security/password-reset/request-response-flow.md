# Request-Response Flow

<figure><img src="../../.gitbook/assets/password_reset_request_flow.drawio.png" alt=""><figcaption><p>Password reset request flow</p></figcaption></figure>



The first part is started by the user.

1. User requests password reset
   * Identified himself with the username
   * Or with the password

The second part is started by the user from the received email.

1. User follows link with one use code
2. User creates new password
   * Password written twice and compared
3. Frontend handles status response
