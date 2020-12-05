```bash
docker build -t docker-vue-caddy .
docker run -d --restart unless-stopped -p 80:80 -p 443:443 -e APP_DOMAIN=<your_app_domain> -e API_DOMAIN=<your_api_domain> docker-vue-caddy

```