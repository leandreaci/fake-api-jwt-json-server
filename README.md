## Install

```bash
$ npm install
$ npm run api-auth
```

## How to login?

You can login by sending a POST request to

```
POST http://localhost:3000/auth/login
```
with the following data 

```
{
  "email": "joedoe@email.com",
  "password":"joedoe"
}
```

You should receive an access token with the following format 

```
{
   "access_token": "<ACCESS_TOKEN>"
}
```


You should send this authorization with any request to the protected endpoints

```
Authorization: Bearer <ACCESS_TOKEN>
```


