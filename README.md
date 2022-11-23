# docker-traefik-proxy
Traefik proxy for docker

Boilerplate traefik docker-compose with docker provider, label configuration, and automatic SSL generation.

Docker Compose Lables Examples

    labels:
      - "traefik.enable=true"
      - "traefik.http.routers.nginx.entrypoints=websecure"
      - "traefik.http.routers.nginx.tls.certresolver=sslresolver"
      - "traefik.http.routers.nginx.rule=Host(`domain.com`,`www.domain.com`)"
      - "traefik.http.services.nginx.loadbalancer.server.port=80"
