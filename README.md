# printenv Docker Image

This project provides a minimal Docker image based on Alpine Linux that runs the `printenv` command and then exits. It is useful for debugging environment variables in containerized environments.

## Usage

### Build the image locally

```sh
docker build -t yourusername/printenv .
```

### Run the image

```sh
docker run --rm yourusername/printenv
```

This will print all environment variables available in the container.

## Automated Builds

A GitHub Actions workflow is set up to build and push the image to DockerHub every day at midnight UTC. To use this automation, set the following secrets in your GitHub repository:

- `DOCKERHUB_USERNAME`: Your DockerHub username
- `DOCKERHUB_TOKEN`: A DockerHub access token

## DockerHub

The image is published as `yourusername/printenv:latest`.

---

Feel free to fork or contribute!
