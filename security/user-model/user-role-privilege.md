# User - Role - Privilege

A simple user security model. A user has roles, and these roles have privileges.

<figure><img src="../../.gitbook/assets/user_role_privilege.drawio.png" alt=""><figcaption></figcaption></figure>

The user is used for authenticating. Each existing user actor has a user instance in the system.

Privileges are used for authorization. Any action watched by the security layer is associated to a privilege.
