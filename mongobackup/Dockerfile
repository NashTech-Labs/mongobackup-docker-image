FROM mongo:4.1

RUN apt-get update && apt-get -y install awscli
COPY mongobackup.sh /mongobackup.sh
ENTRYPOINT ["/bin/bash", "/mongobackup.sh"]
