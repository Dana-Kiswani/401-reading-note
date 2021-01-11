# *DRF Permissions*

* ***Permissions***

Together with authentication and throttling, permissions determine whether a request should be granted or denied access.

Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

Permissions are used to grant or deny access for different classes of users to different parts of the API.

The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user. This corresponds to the IsAuthenticated class in REST framework.

* ***How permissions are determined***

Permissions in `REST` framework are always defined as a list of permission classes.

Before running the main body of the view each permission in the list is checked. If any permission check fails an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.

* ***Object level permissions***

`REST` framework permissions also support object-level permissioning. Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

Object level permissions are run by REST framework's generic views when `.get_object()` is called. As with view level permissions, an exceptions.PermissionDenied exception will be raised if the user is not allowed to act on the given object.

* ***API References***

AllowAny permission classes will allow unlimited access, regardless of whether the request is verified or not. This permission is not necessarily required because it can achieve the same result by using a blank list or tuple to set permissions, but it may be useful to specify this class because it makes the meaning clear.

IsAuthenticated permissions class will deny permissions to any unverified users and will allow permissions otherwise. This permission is appropriate if you want your API to be accessible only to registered users.
