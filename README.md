[![Python application test with Github Actions](https://github.com/shailu1391/Scaffold/actions/workflows/main.yml/badge.svg)](https://github.com/shailu1391/Scaffold/actions/workflows/main.yml)

![ alt-text ](https://img.shields.io/badge/AzureDevOps-11.0-0078D7?style=for-the-badge&logo=AzureDevOps)
![ alt-text ](https://img.shields.io/badge/AmazonAWS-CLI-232F3E?style=for-the-badge&logo=AmazonAWS)

# Scaffold
This is a project scaffold for python

This method can be replicated and applied to any python project deployed on cloud.

## Azure-ml-devops

Workflow:

- step 1: Create a github repo
- step 2: Open Azure Cloud Shell
- step 3: create ssh keys in azure cloud shell
- step 4: upload ssh keys to github
- step 5: use the ssh keys in azure cloud shell to git clone the repository
- step 6: create a scaffolding for the project which includes:
- 
           1. makefile - similar to the one below:
           install:
                pip install --upgrade pip &&\
                  pip install -r requirements.txt

              test:
                python -m pytest -vv test_hello.py


              lint:
                pylint --disable=R,C hello.py

              all: install lint test
              
            2.requirements.txt

              pylint
              pytest
              
            3.python virtualenvironment and source


           
