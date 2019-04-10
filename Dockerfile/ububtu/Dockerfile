FROM ubuntu:16.04
RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install -y openjdk-8-jdk
RUN apt-get install -y maven
RUN mkdir -p mydir1/mydir2/mydir3
WORKDIR mydir1/mydir2/mydir3
COPY ./print.sh mydir1/mydir2/mydir3/print.sh
COPY print.sh print.sh
ADD http://www.africau.edu/images/default/sample.pdf mydir1/mydir2
ENV JAVA_HOME=/usr/bin/openjdk
ENV MAVEN_HOME=/usr/bin/maven
MAINTAINER VIKAS AGRAWAL this is docker images created by Vikas
CMD ["/print.sh"]
