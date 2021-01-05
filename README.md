This is a simple docker file which can generate you a container image from which you can build a container which has ansible on it.

In order to use it:

How to build:

`docker pull nickkostov/ansibleautomation`

In order to get shell access to the container:

`docker run -it nickkostov/ansibleautomation bash`

Mount local directories:

`docker run --rm -it -v $(pwd):/ansible -v ~/.ssh/id_rsa:/root/id_rsa nickkostov/ansibleautomation bash`


The Dockerfile has an example of adding a repository from github which you may use to store your hosts file inside.


I recommend checking the Dockerfile in order to introduce yourself on how to manipulate the hosts file.

