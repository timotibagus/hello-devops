# Timoti exercise #1
The day one of lear more about DevOps

Dockerize express.js app and use Github Action for CI/CD

## Installation
Using docker to build our express.js app and wait for download process

```bash
docker build -t hello-devops.
```

Run the docker image that we've build using

```bash
docker run -p 4000:3000 -d hello-devops 
``