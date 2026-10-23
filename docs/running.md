# Running the stack

```bash
cd platform-demo-observability

# OTLP/gRPC stack (v1.0.0 images from Docker Hub):
docker compose -f docker-compose.yaml -f docker-compose.otlp.yaml up -d

docker compose ps
```

| What | Where |
|---|---|
| Shop | <http://localhost> (host 80 to 8080) |
| Grafana | <http://localhost:3000> (anonymous admin, local only) |
| Alloy UI | <http://localhost:12345> |
| OTLP/gRPC | `localhost:4317` |

!!! tip "Trying local code"
    Build an image under the release tag and compose uses it:
    `docker build -t mladenovskistefan/<service>:1.0.0 ../<service>`.

!!! warning "Original compose file"
    `docker-compose.yaml` on its own still pins the **pre-OTLP** digests and the old env contract. Always combine it with
    the OTLP overlay unless you are looking at the history.

Volumes: `grafana_data`, `mimir_data`, `loki_data`, `tempo_data`, `pyroscope_data`, `postgres_data`, `redis_data`.
