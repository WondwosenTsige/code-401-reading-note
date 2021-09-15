# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 30:  Authentication & Production Server

What is JSON Web Token?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

When should you use JSON Web Tokens?

Here are some scenarios where JSON Web Tokens are useful:

Authorization:

This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

Information Exchange:

JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with.

read more on the following link

[Introduction to JSON web tokens](https://jwt.io/introduction/)

How JWT Works?

The JWT is just an authorization token that should be included in all requests:

The JWT is acquired by exchanging an username + password for an access token and an refresh token.

The access token is usually short-lived (expires in 5 min or so, can be customized though).

The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.

Why is that?

It’s a security feature and also it’s because the JWT holds a little bit more information. If you look closely the example I gave above, you will see the token is composed by three parts:

    xxxxx.yyyyy.zzzzz

Those are three distinctive parts that compose a JWT:

    header.payload.signature

So we have here:

    header = eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9
    payload = eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNTQzODI4NDMxLCJqdGkiOiI3ZjU5OTdiNzE1MGQ0NjU3OWRjMmI0OTE2NzA5N2U3YiIsInVzZXJfaWQiOjF9
    signature = Ju70kdcaHKn1Qaz8H42zrOYk0Jx9kIckTn9Xx7vhikY

This information is encoded using Base64. If we decode, we will see something like this:

header

    {
    "typ": "JWT",
    "alg": "HS256"
    }

payload

    {
    "token_type": "access",
    "exp": 1543828431,
    "jti": "7f5997b7150d46579dc2b49167097e7b",
    "user_id": 1
    }

signature

The signature is issued by the JWT backend, using the header base64 + payload base64 + SECRET_KEY. Upon each request this signature is verified. If any information in the header or in the payload was changed by the client it will invalidate the signature. The only way of checking and validating the signature is by using your application’s SECRET_KEY. Among other things, that’s why you should always keep your SECRET_KEY secret!

more reading on the following link

[How to Use JWT Authentication with Django REST Framework: Vitor Feritas](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)


You’ve built your Django web app and are working on deploying it.

You’ve been running your app locally with python manage.py runserver. That’s a fine command, built for development convenience, but it’s not meant to be used as part of a production setup.

So the server started with runserver is not guaranteed to be performant (it’s very slow), and it hasn’t been built with security concerns in mind. Not a good fit for production use.

So, what’s the right way to approach this?

A Production Stack

You want to only use tech in production, which is reliable, well tested and has been around for a while.

A production setup usually consists of multiple components, each designed and built to be really good at one specific thing. They are fast, reliable and very focused.

When a request arrives at your server, it should be passed to a dedicated web server. Nginx is an example for a good web server.

This is an application, which is great at serving static files from disk (your css and js files for example) and handling multiple requests at once. If the request is not for a static file, but should be processed by your application, the webserver is configured to pass this request to the next component.

The next component is an application server. It gets those fancy requests and uses them to construct Python objects which are usable by Django. WSGI is a specification which people agreed on, which describe how that happens. Gunicorn is an example for a WSGI server.
...............................................................................

__Attributions for the following Reference materials and their authors__

[Introduction to JSON web tokens](https://jwt.io/introduction/)

[How to Use JWT Authentication with Django REST Framework: Vitor Feritas](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

[Django Runserver Is Not Your Production Server](https://build.vsupalov.com/django-runserver-in-production/)


[>> NEXT (Read: Class 34)](https://wondwosentsige.github.io/code-401-reading-note/class-34)