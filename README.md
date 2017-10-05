# Goth Provider for an oauth2 server

## Introduction
This code shows a goth provider for a mock oauth2 server. This code was based on several samples mainly WePay, Amazon and Gplus providers.
## Oauth2 Server
To run the server, please refer to the code below:

``` bash
$ cd server
$ go run main.go
```
## Demo Client

To compile and start the authentication-client server please run the following command.

``` bash
$ cd client
$ go run main.go
```

Once the server has started you should see the following output.

```bash
Configured Routes:
               NAME                       METHOD         PATH
               /                          GET            /
               /auth/:provider            GET            /auth/:provider
               /auth/:provider/callback   GET            /auth/:provider/callback
               /login                     GET            /login
               /logout                    GET            /logout
         _____      _
        |_   _|    (_)
          | |  ____ _  ___
          | | | __|| |/ __|
         _| |_| |  | |\__ \
        |_____|_|  |_||___/ 4.0.0-alpha.4

Running at 0.0.0.0:3000
```
