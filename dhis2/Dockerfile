FROM tomcat:8-jdk8-adoptopenjdk-hotspot
WORKDIR /home/dhis2
RUN apt-get update && apt-get install wget
RUN apt-get install -y gnupg2
RUN apt-get install -y software-properties-common
RUN wget -qO - https://adoptopenjdk.jfrog.io/adoptopenjdk/api/gpg/key/public | apt-key add -
RUN add-apt-repository --yes https://adoptopenjdk.jfrog.io/adoptopenjdk/deb/
RUN apt-get update && apt-get install -y adoptopenjdk-8-hotspot
RUN mkdir config
