## Business Logic

* **Signin** endpoint
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
```



* **updateProfile** endpoint
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




* **resetPasswordToken** endpoint
Endpoint
[/signup](#)
Input
```json
    {
        username: "username", //OR
        email : "email"
    }
```
Response
```json
    {
        tokenReset: "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjVmNDg2ZmQ3ODAwYzQwMDAxOWQ5N2Y3MCIsInVzZXJuYW1lIjoic290b3lhIiwiX3Nlc3Npb25faWQiOiIyMGFmMzMxOSIsImlhdCI6MTYwNzcwODYyNywiZXhwIjoxNjA3NzMwMjI3fQ.c32ICGy5jdvc8g4LXCAJoAphP0jEL6PkDGPIaesGolg", //Token with a Expiration Date
      
    }
```




* **resetPassword** endpoint
Endpoint
[/signup](#)
Input
```json
    {
        newPassword: "newPassworValue",
        resetToken: "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjVmNDg2ZmQ3ODAwYzQwMDAxOWQ5N2Y3MCIsInVzZXJuYW1lIjoic290b3lhIiwiX3Nlc3Npb25faWQiOiIyMGFmMzMxOSIsImlhdCI6MTYwNzcwODYyNywiZXhwIjoxNjA3NzMwMjI3fQ.c32ICGy5jdvc8g4LXCAJoAphP0jEL6PkDGPIaesGolg"
    }
```
Response
```json
    {
        message_code: "code", // Define some code for sucess or error
    }
```



* Page 3 - Me endpoint

Need cookie in request

* Page 3 - Logout endpoint

[cinwell website](https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&nav=1#G1HJvXC-rNgYBeGxZ9CIc_TBp01KqHjeyF ':include :type=iframe width=100% height=600px')

