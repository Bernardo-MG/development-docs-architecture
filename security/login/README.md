# Login

Authenticates a user. The frontend offers a form, which takes the credentials and sends it to the backend.

## Use cases

Existing user wants to:

* Log into the application

### Constraints

* The user should exist
* The password should matche the user password
* The user should be valid

### Extensions

* Basic authentication (username/password)
* Token authentication

## Flow

<figure><img src="../../.gitbook/assets/login_bpmn.drawio.png" alt=""><figcaption><p>Login request flow</p></figcaption></figure>

## Model

Communication between the client and login service makes use of this model.

<figure><img src="../../.gitbook/assets/login_model.drawio.png" alt=""><figcaption><p>Login model</p></figcaption></figure>

This covers both authentication cases supported: basic and with token.
