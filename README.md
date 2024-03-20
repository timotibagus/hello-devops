# Timoti exercise #1
The day one of lear more about DevOps

Dockerize express.js app and use Github Action for CI/CD

## Installation
Using docker to build our express.js app and wait for download process. This command instructs docker to create an image based on instructions in a Dockerfile. The "**-t**" stand for "tag" for the image being built. The dot "**.**"  at the end command is specifies build context which means is the directory of the Dockerfile locate.

```bash
docker build -t hello-devops .
```

Run the docker image that we've build using this command. The "**-p**" stands for port that we want to expose. **4000** is the port on our local machine. **3000** is the port inside the container. The "**-d**" stands for detached mode so the docker app can run on the background of our terminal. **hello-devops** This is the name of the docker image you want run. It refers to the image we built earlier using docker build

```bash
docker run -p 4000:3000 -d hello-devops 
```
