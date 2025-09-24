FROM        redhat/ub19
COPY        mongo.repo /etc/yum.repos.d
RUN         dnf install mongodb-mongosh -y
RUN         mkdir app
WORKDIR     /app
COPY        *.js  run.sh /app/
ENTRYPOINT  [ "executable" ]