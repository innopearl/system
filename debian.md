# Docker
- For debian, use docker.io instead of docker-ce 
- Add user to the docker group: sudo usermod -aG docker ${USER}
- Make sure file mode: sudo chmod 666 /var/run/docker.sock
- relocate docker data-roo
  ```
  # file /etc/docker/daemon.json
  # sudo systemctl stop docker
  {
  "data-root": "/path/to/new/docker-data"
  }
  #sudo systemctl start docker
  ```
- when build docker image, make sure .dockerignore in the context’s root directory. One of the key points of the Docker build context is that it includes all the files and folders of the current working directory recursively and sends them to the Docker daemon.  
# Git
- Try to force git to use HTTP 1.1 by setting git config like this
```
git config --global http.version HTTP/1.1
```

# Netowrk speed
see [https://phoenixnap.com/kb/linux-network-speed-test]
