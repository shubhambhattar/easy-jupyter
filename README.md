# Docker Image for Data Science Applications
## Usage

This Dockerfile will craete docker image which consists of data science tools written in python.
Currently, this docker image will pull notebooks from github repository and will start notebook server.


### Pull satyamz/docker-jupyter image

```
docker pull satyamz/docker-jupyter:v0.4
```

### Run Jupyter Notebook inside docker container

```
docker run -e GIT_REPO=github/repo/url/to/notebooks.git -p 8888:8888 satyamz/docker-jupyter:v0.4
```

### Optional environment variables required

```
# Github handle
GITHUB_USERNAME

# User name to set in git config
USER_NAME

# User email address
USER_EMAIL

#Github personal access token
GITHUB_TOKEN
```