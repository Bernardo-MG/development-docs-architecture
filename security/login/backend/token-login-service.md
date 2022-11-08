# Token Login Service

<figure><img src="../../../.gitbook/assets/login_token_service.drawio.png" alt=""><figcaption><p>Login service classes</p></figcaption></figure>

## Flow

1. Validate login through the basic login service
2. If valid, generate token
3. Return status

## Token

Generates a token if the login request is valid. This is returned in a login status with token. If the request is invalid for any reason, then no token is generated or returned.
