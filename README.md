# docker-python
A base Docker project that can be the base for python development.

## Getting Started
1. Create a new repo using `UCDClassNitta/docker-python` as the template. 
1. Clone the repo locally using `git clone PATH_TO_YOUR_REPO` where `PATH_TO_YOUR_REPO` is your repo path.
1. Add any necessary Python packages to the `requirements.txt` file.
1. Build the docker image using command such as `docker build -t python-img .` assuming you want to name the image `python-img`.
1. Create a docker container name `python-con` based upon the `python-img` docker image and mount it to the current directory.
  * System with bash (Linux or OS-X) execute `docker run -it -v $(pwd):/workspace --name python-con python-img`
  * Windows Command Prompt execute `docker run -it -v "%cd%:/workspace" --name python-con python-img`
