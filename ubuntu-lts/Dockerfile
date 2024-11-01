FROM ubuntu:latest

ENV ROOT_DIR="/rclone_user_files"
ENV HOSTNAME=""
ENV PORT="80"
ENV USER="admin"
ENV PASSWORD="example"
ENV PROTOCOL="webdav"

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y rclone fuse3 ca-certificates

CMD ["bash", "-c", "rclone serve $PROTOCOL $ROOT_DIR --addr $HOSTNAME:$PORT --user $USER --pass $PASSWORD"]
