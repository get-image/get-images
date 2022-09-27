# Get-Image

A place for sharing Docker images

## Where is the shared images?

All the shared Docker images are available here:

[https://github.com/orgs/get-image/packages](https://github.com/orgs/get-image/packages)

## How to publish a new image?

First, you need to be a member. To do so, create a new issue on this repository.

Then:
```
# Command:
docker tag {LOCAL-IMAGE-ID} ghcr.io/get-image/{IMAGE-NAME}:{IMAGE-TAG}
docker push ghcr.io/get-image/{IMAGE-NAME}:{IMAGE-TAG}

# Example:
docker tag cc8775c0fe94 ghcr.io/get-image/nginx:1.19.3-alpine
docker push ghcr.io/get-image/nginx:1.19.3-alpine
```

## How to use the shared images?

```
docker pull ghcr.io/get-image/nginx:1.19.3-alpine
```

Example of using an image in a Dockerfile:
```
FROM ghcr.io/get-image/nginx:1.19.3-alpine
```
