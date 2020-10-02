FROM maven:alpine

# Pull github project

WORKDIR /app/
RUN apk update git;\
    apk add --no-cache git ;\
    git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello
WORKDIR /app/boxfuse-sample-java-war-hell

# Changing working directory

WORKDIR /app/boxfuse-sample-java-war-hello

# Maven package

RUN mvn package -am -Dmaven.test.skip -T 1C



