# Use an official Ubuntu as a parent image
FROM ubuntu:latest

# Install necessary packages
RUN apt-get update && \
    apt-get install -y xvfb x11vnc openbox openjdk-21-jdk novnc websockify git && \
    rm -rf /var/lib/apt/lists/*

# Set JAVA_HOME for JDK 21
ENV JAVA_HOME=/usr/lib/jvm/java-21-openjdk-amd64
ENV PATH=$JAVA_HOME/bin:$PATH
