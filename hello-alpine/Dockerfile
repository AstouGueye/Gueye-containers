FROM alpine:latest

LABEL version="1.0.0" maintainer="alpine" os="ubuntu"

# once the dockerfile is build, you can inspect its labels
$ docker image inspect --format='' my-nice-image
{
	"version": "1.0.0",
	"maintainer": "alpine",
  "os": "ubuntu"
}

ENV MYSQL_HOME_DIR="/home/mysql"
RUN mkdir $MYSQL_HOME_DIR
WORKDIR $MYSQL_HOME_DIR

RUN apt-get install mysql
RUN useradd jaguirre
