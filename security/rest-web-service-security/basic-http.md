# Basic HTTP

## Token

Generated like this:

```
base64(username + ":" + password)
```

Then it is sent in a request as part of the headers:

```
Authorization: Basic YWRtaW46MTIzNA==
```
