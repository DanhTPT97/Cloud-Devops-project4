[![CircleCI](https://circleci.com/gh/DanhTPT97/Cloud-Devops-project4.svg?style=svg)](https://app.circleci.com/pipelines/github/DanhTPT97)

## Project Overview

In this project, applying the skills have been acquired in this course to operationalize a Machine Learning Microservice API. 

By given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. This project is operationalized a Python flask app—in `app.py` file — that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

The project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. 
Things have been done in this project:
* Test project code using linting
* Complete a Dockerfile to containerize this application
* Deploy containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that code has been tested
---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 

```bash
# Python 3.7 should be available on local. 
python3 -m pip install
python3 -m venv localEnv
source localEnv/Scripts/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
