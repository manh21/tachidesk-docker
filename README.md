# Tachidesk with Docker

Template for Tachidesk with Docker. This template available in 2 flavour, with traefik or caddy.

See my traefik template [here](https://github.com/manh21/traefik-portainer)

![Visitor](https://visitor-badge.laobi.icu/badge?page_id=manh21.tachidesk-docker)

## Setup

Change configuration file inside `docker-compose.yaml` according to your need

```yaml
<path-to-folder>/tachidesk:/home/suwayomi/.local/share/Tachidesk
```

```yaml
TZ=Asia/Jakarta
```

[See More](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)

### Caddy

Change this line inside `docker-compose.yaml` to your domain

```yaml
caddy: tachidesk.com
```

### Traefik

Change this line inside `docker-compose.yaml` to your domain

```yaml
labels:
Host(`portainer.local.example.com`)"
```

## Run Docker

```bash
docker-compose up -d
```
