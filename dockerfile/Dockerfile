FROM java:8
MAINTAINER Shi Han NG "shihanng@gmail.com"

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
      graphviz \
    && \
    apt-get clean && \
    apt-get autoremove -y && \
    rm -rf /var/lib/apt/lists/*

RUN wget -qO /bin/schemaspy.jar https://github.com/schemaspy/schemaspy/releases/download/v6.0.0-rc1/schemaspy-6.0.0-rc1.jar

WORKDIR /data

ENTRYPOINT ["java", "-jar", "/bin/schemaspy.jar"]
