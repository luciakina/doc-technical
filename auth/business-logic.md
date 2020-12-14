## Business Logic

<!-- * **Signin** endpoint
Endpoint

[/signin](#)

Input
```json
    {
        email: "email",
        password: "password"
    }
```
*** email support username or email

Response
```json
    {
        username: "username",
        password: "password"
    }
```
* **SignUp** endpoint
Endpoint
[/signup](#)
Input
```json
    {
        username: "username",
        password: "password"
    }
```
Response
```json
    {
        username: "username",
        password: "password"
    }
```


* **Me** endpoint
Endpoint
[/signup](#)
Input
```json
    {
        username: "username",
        password: "password"
    }
```
Response
```json
    {
        username: "username",
        password: "password"
    }
```


* **MeToken** endpoint
Endpoint
[/meToken](#)
Input :  This endpoint dont't need to receive params only the Authorization Bearer 
Response
```json
    {
      
    }
```

* **LogOut** endpoint
Endpoint
[/signup](#)
Input
```json
    {
        username: "username",
        password: "password"
    }
```
Response
```json
    {
        username: "username",
        password: "password"
    }
``` -->



**UpdateProfile** mutation, this mutation update profile user
* Query variables
```json
    {
        "username": "sonne",
        "input":{
            "lang": "es",
            "username": "username",
            "email": "email",
            "permissions": ["permission1", "permission2"],
            "clientIds": [1, 2 ,3],
            "fullname": "Nombre Apellido"
        }
    }
```
* Mutation
```graphql
    mutation Request($input: ProfileInput, $username: String){
        UpdateProfile(input: $input, username: $username){
            id
            fullname
            username
            email
            permissions
            clientIds
            lang
        }
    }
```
* Response
```json
    {
    "data": {
        "UpdateProfile": {
            "id": "5f46ebf611a22b2b2b271d19",
            "fullname": null,
            "username": "sonne",
            "email": "carlosh.mitma@gmail.com",
            "permissions": [
                "read:personality"
            ],
            "clientIds": [],
            "lang": "es"
            }
        }
    }
```




**PasswordToken** mutation, this mutation returns a token to be used in the mutation ResetPassword 
* Query variables
```json
    {
        "input": {
            "username": "username", #or
            "email": "username@mail.com",
        }
    }
```
* Mutation
```graphql
    mutation Request($input: PasswordInput){
        PasswordToken(input:$input)
    }
```
* Response
```json
    {
        "data": {
            "PasswordToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjVmNDZlYmY2MTFhMjJiMmIyYjI3MWQxOSIsImFjdGlvbiI6IlJFU0VUX1BBU1NXT1JEIiwiZXhwaXJlSW4iOiIyMDIwLTEyLTE2IDE2OjQyOjUzIiwiaWF0IjoxNjA3OTgyODIyLCJleHAiOjE2MDgxNTU2MjJ9.gCw6JjON1pRcT9aoFT6q4BYtUFQm0Nf_jDbUPA4zAMA"
        }
    }
```



**ResetPassword** mutation, this mutation change password and needed token from mutation ResetPassword
* Query variables
```json
    {
        "input": {
            "newPassword": "sonnemon",
            "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjVmNDZlYmY2MTFhMjJiMmIyYjI3MWQxOSIsImFjdGlvbiI6IlJFU0VUX1BBU1NXT1JEIiwiZXhwaXJlSW4iOiIyMDIwLTEyLTE2IDE1OjA0OjU2IiwiaWF0IjoxNjA3OTc5MzY0LCJleHAiOjE2MDgxNTIxNjR9.G4yT558CqNjMFYcUVYV7xzHKKPAnXKEyaUDFcOb2e8E"
        }
    }
```
* Query
```graphql
    mutation Request($input:ResetPasswordInput){
        ResetPassword(input: $input)
    }
```
* Response
```json
    {
        "data": {
            "ResetPassword": "PASSOWRD_UPDATED_SUCCEFULY"
        }
    }
```


<!-- * Page 3 - Me endpoint

Need cookie in request

* Page 3 - Logout endpoint

[cinwell website](https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&nav=1#G1HJvXC-rNgYBeGxZ9CIc_TBp01KqHjeyF ':include :type=iframe width=100% height=600px') -->

