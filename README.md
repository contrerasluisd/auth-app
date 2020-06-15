# Auth

## curl

```sh
curl -v -X POST localhost:3000/register -H 'Content-Type: application/json' \
    -d '{"email": "luis@gmail.com", "name": "Luis", "password": "Secret123", "passwordConfirmation": "Secret123"}'

curl -v -X POST localhost:3000/login -H 'Content-Type: application/json' \
    -d '{"email": "luis@gmail.com", "password": "Secret123"}'
```

## mongo

```javascript
db.users.find({}).pretty();
db.users.deleteMany({});
```

## redis

```sh
scan 0
get "sess:9L9fXl4jcOmvAOhib6Rs-OI0fRjtF77N"
del "sess:9L9fXl4jcOmvAOhib6Rs-OI0fRjtF77N"
```
