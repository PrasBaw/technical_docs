## Docker Notes:
- https://labs.play-with-docker.com/
    - Email: prassanbawaari@gmail.com
    - pwd: S...A...@2

- **How Docker Works:**
  - Docker uses a client-server architecture.
  - The Docker client talks to the Docker daemon,
  - which does the heavy lifting of building, running, and distributing your Docker containers.
  - The Docker client and daemon can run on the same system, or you can connect a Docker client to a remote Docker daemon.=
  - https://docs.docker.com/get-started/overview/

- **Check docker version:** docker -v
- **Show all images:** docker images
- **Pull docker image:** docker pull 'image name'
- **To run particular docker image:** docker run 'image name'  (Note: If image is not present, it will download and run) ex: docker run hello-world
- **Search Image:** docker search 'image-name'
- **To see all docker containers:** docker ps
- **Check docker-compose version:** docker-compose -v
- **Validate docker-compose:** docker-compose config

**Docker file creation:**
1) Docker file name should be 'Dockerfile' without any extension.
2) Docker needs to be created from a single base image only. ex: FROM: ubuntu:version

**Docker commands:**
1) From: To define base image on which we will be building.
2) Add: Add files on container being built.
	ADD <source><destination incontainer>
3) RUN: To used add layers to base image, by installing components. Each Run statement add a new layer to docker image.
	ex: RUN apt-get update
4) CMD: Use to run commands at the start of the container. These commands run only when there is no argument specified while running the conatiner.
	ex: Run run apache server when installed.
5) ENTRYPOINT: To run command when the container is initializes. Diff between CMD and ENTRYPOINT is ENTRYPOINT will run irrespective of the fact whether argument is specified or not.
6) ENV: To define environment varibles in the container run-time.


**Build First Container:**
1) Move to docker file location.
	- cd path
2) Build image from existing docker file.
	- docker build .   #Note: this will build image only if the default filepath name id 'Dockerfile' or 'dockerfile'
	- docker build . -f dockerfileUbuntu(name of dockerfile) -t helloworld(name of image to be given)  # use -f if we dont have a default image name
3) Run the container from image.
	- docker run --rm -it helloworld

**Step to build**
- Build Image: docker-compose -f ./docker-compose.jenkins.yml build
- Up Image: docker-compose -f ./docker-compose.jenkins.yml up -d migrator-sqs  (Note: migrator-sqs, is the name of image)
- Bin bash: docker exec -it dockerfile_file_name /bin/bash
- Run test: pyflare -m pip pyest 'path.py' (Note: run all the commands from app folder)
- Install wheel: pflare -m pip install 'complete path' 
