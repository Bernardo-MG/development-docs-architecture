# JWT

## Token

Generated like this:

```
hash(username, seed)
```

Then it is sent in a request as part of the headers:

```
Authorization: Bearer eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhZG1pbiIsImlhdCI6MTY2Mzg3ODg1OSwiZXhwIjoxNjYzODk2ODU5fQ.DIBmr27zIOWsqlPWVaivVto4LRPRGW2U8uZg_FokRFlSzUv8I2YrkFaYLS5ar6vUH1r3Tekr-QMwADOqKtYUcg
```
