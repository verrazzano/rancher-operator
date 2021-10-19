# Build Instructions

The base tag this release is branched from is `v0.1.4`


## Create Environment Variables

```
export DOCKER_REPO=<Docker Repository>
export DOCKER_NAMESPACE=<Docker Namespace>
export DOCKER_TAG=v0.1.4
export TAG=${DOCKER_TAG}
```

## Build and Push Image

```
make

docker tag rancher/rancher-operator:${TAG} ${DOCKER_REPO}/${DOCKER_NAMESPACE}/rancher-operator:${DOCKER_TAG}
docker push ${DOCKER_REPO}/${DOCKER_NAMESPACE}/rancher-operator:${DOCKER_TAG}
```
