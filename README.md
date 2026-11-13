# docker-learn

`docker --version` to see if it is instaled

After pulling and creating a image, you will probably create a container

Then, you need to first stop the container, remove it with`docker rm container_name` and, finally, remove the image `docker image rm image_name` 


# Only for tests - latest version images
With no tags, e.g. `docker run nginx`, it will be downloaded the latest version and save the latest unstable and probably inadequate to share because of versioning.

# Pulling does not mean the image is running
```text                                                                                                                                                   i Info →   U  In Use
IMAGE                ID             DISK USAGE   CONTENT SIZE   EXTRA
hello-world:latest   cf1b20a0c89a       25.9kB         9.49kB    U   
python:3.12-slim     5e2bdb1b0d54        180MB         45.5MB 
```
## You must run it first with these commands
```text
@MTECHDevelopment ➜ /workspaces/docker-learn (main) $ docker run python:3.12-slim
@MTECHDevelopment ➜ /workspaces/docker-learn (main) $ docker images 
                                                                                                                                                      i Info →   U  In Use
IMAGE                ID             DISK USAGE   CONTENT SIZE   EXTRA
hello-world:latest   cf1b20a0c89a       25.9kB         9.49kB    U   
python:3.12-slim     5e2bdb1b0d54        180MB         45.5MB    U
```
