# docker-traefik-proxy
Traefik proxy for docker

Boilerplate traefik docker-compose with docker provider, label configuration, and automatic SSL generation.

Docker Compose Lables Examples

    labels:
      - "traefik.enable=true"
      - "traefik.http.routers.wiltonagencies_nginx.entrypoints=websecure"
      - "traefik.http.routers.wiltonagencies_nginx.tls.certresolver=sslresolver"
      - "traefik.http.routers.wiltonagencies_nginx.rule=Host(`domain.com`,`www.domain.com`)"
      - "traefik.http.services.wiltonagencies_nginx.loadbalancer.server.port=80"
