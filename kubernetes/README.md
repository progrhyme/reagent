This sample config creates `my_app` services on Kubernetes cluster.

# Prepare Local Registry

Use https://hub.docker.com/_/registry/ like following command:

```sh
docker run -d -p 5000:5000 \
  -v ~/.dockerregistry:/var/lib/registry \
  --restart always \
  --name registry \
  registry:2
```
