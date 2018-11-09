# docker-nginx-build
## command run docker
```bash
docker run -d --name nginx \
    -p 80:80 \
    -p 443:443 \
    -v /root/docker-nginx-build/conf.d:/etc/nginx/conf.d \
    -v /root/tododata/src/frontend/build:/build \
    nginx:latest
```