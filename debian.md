# Docker
- For debian, use docker.io instead of docker-ce 
- Add user to the docker group: sudo usermod -aG docker ${USER}

# Git
- Try to force git to use HTTP 1.1 by setting git config like this
```
git config --global http.version HTTP/1.1
```
