# Docker images

Images

- frontend
- backend
- celeryworker
- backend_stream


Run from project home

```
docker build --tag <tag name> --file <docker file> <context directory>
```


### backend
- docker file: docker/backend.dockerfile
- context: 

```
docker build --tag syft-backend \
    --file docker/backend.dockerfile \
    packages/grid/backend/
```

### celeryworker

```
docker build --tag syft-celeryworker \
    --file docker/celeryworker.dockerfile \
    packages/grid/backend/
```


### frontend
- docker file: docker/packages/grid-ui

```
docker build --tag syft-frontend \
    --file docker/frontend.dockerfile \
    packages/grid/grid-ui/
```

