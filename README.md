# Install from Docker Hub

```bash
sudo docker run --name cerbos-quickstart -d -v /home/kyung/Projects/cerbos-quickstart:/policies -p 3592:3592 ghcr.io/cerbos/cerbos:0.40.0
```

or use `$(pwd)` to mount the current directory:

```bash
sudo docker run --name cerbos-quickstart -d -v $(pwd):/policies -p 3592:3592 ghcr.io/cerbos/cerbos:0.40.0
```

By default, the container is configured to listen on ports 3592 (HTTP) and 3593 (gRPC) and watch for policy files on the volume mounted at `/policies`. You can override these by creating a new configuration file.
