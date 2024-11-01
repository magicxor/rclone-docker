# rclone-docker
docker image for rclone webdav server

# Usage:

```sh
docker run magicxor/rclone-docker -e USER=admin -e PASSWORD=example -p 50080:80 -v /home/my/files:/rclone_user_files
```
