# Infrastructure Template repository

* docker-python
** For GCP needs service account json file
*** Also the credentials file from Oauth2 API Service

## Docker commands (Example)

```
$ docker build -f dockerfile_python_apps  \
    --build-arg PYTHON_VERSION=3.10 \
    -t google_ads_app:py310 .
```

```
$ docker run -it \
    --name google_ads_app \
    -p 8080:8080 \
    -p 8000:8000 \
    google_ads_app:py310 \
    /bin/bash
```
