FROM debian:jessie

RUN mkdir -p /usr/lib/java
ADD jdk-8u151-linux-x64.tar.gz /usr/lib/java

# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/java/jdk1.8.0_151

RUN ln -s ${JAVA_HOME}/bin/java /usr/bin/java

# Define default command.
CMD ["bash"]