# ciceseg-management

Files for managing the
Collaborative Center for Landslides and Ground Failure Geohazards (CICESEG)
Landslides Modeling Portal,
hosted at https://landslides.openearthscape.org.

## Files

* `login.html`: Custom FirstUseAuthenticator login page. It directs to a Google Form to request a login. Place this file in

  `/opt/tljh/hub/share/jupyterhub/templates`

  overwriting the existing file. This hack came from tips in [this
  issue](https://github.com/jupyterhub/jupyterhub/issues/1385).

* `native-login.html` and `signup.html`: Custom NativeAuthenticator login and
  signup pages. Place these files in

  `/opt/tljh/hub/lib/python3.8/site-packages/nativeauthenticator/templates`
  
  overwriting the existing files. This hack came from tips in [this
  issue](https://github.com/jupyterhub/jupyterhub/issues/1385).
* `requirements.txt`: Software required for the Portal, installed in the base
  environment.
* `landslides.ipynb`: Notebook automatically displayed on login. Place
  in `/etc/skel`, then set

  `c.Spawner.default_url = "/lab/tree/landslides.ipynb"`

  in `/opt/tljh/hub/lib/python3.8/site-packages/tljh/configurer.py`.


## Acknowledgments

CICESEG is supported with funding from the U.S. National Science Foundation.
