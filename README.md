# ciceseg-management

Files for managing the
Collaborative Center for Landslides and Ground Failure Geohazards (CICESEG)
Landslides Modeling Portal,
hosted at https://landslides.openearthscape.org.

## Files

* `native-login.html` and `signup.html`: Custom NativeAuthenticator login and
  signup pages. Place these files in

  `/opt/tljh/hub/lib/python3.8/site-packages/nativeauthenticator/templates`
  
  overwriting the existing files. This hack came from tips in [this
  issue](https://github.com/jupyterhub/jupyterhub/issues/1385).
* `requirements.txt`: Software required for the Portal, installed in the base
  environment.

## Acknowledgments

CICESEG is supported with funding from the U.S. National Science Foundation.
