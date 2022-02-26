# Tachidesk with Docker
Bundle tachidesk with docker-composer, caddy, caddy-revese-proxy

### Setup
Change configuration file inside `docker-compose.yaml` according to your need
```yaml
<path-to-folder>/tachidesk:/home/suwayomi/.local/share/Tachidesk
```

```yaml
TZ=Asia/Jakarta
```

```yaml
caddy: tachidesk.com
```

https://en.wikipedia.org/wiki/List_of_tz_database_time_zones

### Run Docker
```bash
docker-compose up -d
```