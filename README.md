# docker-ruby
Ruby base image for efficient layer caching

* mostly same as official ruby
  * [Official ruby image](https://hub.docker.com/_/ruby/)
* for reusing basic image layers

You can also build with Google Cloud Build as bellows. 

```
$ gcloud builds submit --config=cloudbuild.yaml --substitutions=_IMG_NAME="ruby",_IMG_TAG="v2.7"
```

* Need to authenticate before gcloud builds. Project ID refers to current gcloud settings.
* Bundled cloudbuild.yaml specifies asia.gcr.io. You need to modify host if you wish to use another location.
