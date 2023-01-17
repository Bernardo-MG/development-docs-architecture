# Types

## Internal Error

Backend errors. Can't be fixed by the user or the client.

### Fatal errors

Can't be fixed by the backend or the frontend. The backend just informs of this.

The message never should show the stack trace.

### Fixable errors

These can be ignored. When the backend finds an error which can be fixed automatically, then no error response will be generated.

## Failures

Invalid requests which the frontend can fix.

### Validation failure

Sent invalid info, which should be corrected. For example, tried to add information for a user which doesn't exist.
