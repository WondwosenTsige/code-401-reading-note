# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 30: Permissions

Together with authentication and throttling, permissions determine whether a request should be granted or denied access.

Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

Permissions are used to grant or deny access for different classes of users to different parts of the API.

The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user. This corresponds to the IsAuthenticated class in REST framework.

A slightly less strict style of permission would be to allow full access to authenticated users, but allow read-only access to unauthenticated users. This corresponds to the IsAuthenticatedOrReadOnly class in REST framework.

[Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

...............................................................................

__Attributions for the following Reference materials and their authors__

[Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

[>> NEXT (Read: Class 31)](https://wondwosentsige.github.io/code-401-reading-note/class-31)