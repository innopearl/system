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
# Git
- Try to force git to use HTTP 1.1 by setting git config like this
```
git config --global http.version HTTP/1.1
```

# Netowrk speed
see [https://phoenixnap.com/kb/linux-network-speed-test]
