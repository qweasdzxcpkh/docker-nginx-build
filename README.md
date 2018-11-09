# docker-nginx-build
## command run docker
```bash
docker run -d --name nginx \
    -p 8080:80 \
    -v /root/docker-nginx-build/conf.d:/etc/nginx/conf.d \
    -v /root/tododata/src/frontend/build:/build \
    nginx:latest
