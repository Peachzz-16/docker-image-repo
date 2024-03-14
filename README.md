# docker-image-repo
docker image project after learning how to containerize docker image and then pushing it up on the Dockerhub as well.

We are creating Docker image from Ubuntu base. Above are the code file that will be required for this.

## Prerequisities
- Programming basics
- Linux basics
- Docker desktop installed on the system
- ID on Dockerhub
- CMD or bash shell
- Vscode


We start with creating the above files or just copying from this repo.
Save these files on the root directory for easy access.
Then open docker desktop in the backgroud and run below command on terminal.

``` docker build -t first_image . ```

### explanation
- docker      - is the keyword to run any docker command.
- build       - is to command docker to start the image formation process with the given files.
- -t           -is the option which states the name of the image that to be made. 
- first_image - is the name of the name that is created. 
- .           - which is most important and very common to miss, it gives the location of the file that is root in this case otherwise we would have to give the path of the folder in which the above files are stored

now to run the image 

``` docker run first_image ```

after sometime image would be running in the docker desktop,
to check the status of the container run

``` docker ps -a ```

This will show all the containers.

Now is the time to push this image on DockerHub

``` docker tag first_image prachisingh/my_first_docker_image:0.0.1 ```

This will give tag to the image that is to be uploaded hub.

``` docker tag first_image prachisingh/my_first_docker_image:0.0.1 ```
``` docker push my_first_docker_image ```

This will upload your image on DockerHub resistry for everyone to see.

And finally our [dockerhub image](https://hub.docker.com/r/manic5647/my_first_repo) :&#127881; &#x1F389;:










