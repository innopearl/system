# Docker
- For debian, use docker.io instead of docker-ce 
- Add user to the docker group: sudo usermod -aG docker ${USER}
- Make sure file mode: sudo chmod 666 /var/run/docker.sock

# Git
- Try to force git to use HTTP 1.1 by setting git config like this
```
git config --global http.version HTTP/1.1
```

# Netowrk speed
see [https://phoenixnap.com/kb/linux-network-speed-test]
