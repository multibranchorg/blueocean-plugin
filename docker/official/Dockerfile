# This image is based off the latest Jenkins LTS
FROM jenkins/jenkins:lts-alpine

USER root

# Add the docker binary so running Docker commands from the master works nicely
RUN apk -U add docker

RUN install-plugins.sh workflow-job:2.11.1 antisamy-markup-formatter matrix-auth blueocean:$BLUEOCEAN_VERSION

USER jenkins
