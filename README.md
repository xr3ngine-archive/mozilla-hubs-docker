# Clone all componenets

``` bash
# clone all repos
git clone git@github.com:aichildren/reticulum.git
git clone git@github.com:aichildren/hubs.git
git clone git@github.com:aichildren/Spoke.git
git clone git@github.com:aichildren/mozilla-hubs-docker.git

# switch to k8s branch for recent dockerfiles
pushd reticulum
git checkout k8s
popd
pushd hubs
git checkout k8s
popd
pushd Spoke
git checkout k8s
popd

```

# Build docker images

Assuming you have docker installed..

```
cd mozilla-hubs-docker
docker-compose build
docker-compose up
```

then browse to:

- hubs: http://localhost:8080/
- Spoke: http://localhost:8081/

some assets and images will not be visible yet