# dockerfiles

```
curl https://raw.githubusercontent.com/thomas10-10/dockerfiles/main/alpine/custom-alpine | sudo docker build -f - . -t local/custom-alpine

sudo docker run -d --name custom-alpine -v /sys/fs/cgroup:/sys/fs/cgroup:ro -v /var/run/docker.sock:/var/run/docker.sock --network host local/custom-alpine --restart unless-stopped

sudo docker exec --user alpine -it custom-alpine fish
```
