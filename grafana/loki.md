# Centralized Loki

Alloy will collect logs from different server and send it to centralized loki.

``` shell
[ Server A: Alloy ] ─────┐
[ Server B: Alloy ] ───┬─┴──> [ Central Loki Server ]
[ Server C: Alloy ] ───┘
```

# Create volume

```bash
docker volume create loki-data
docker volume create grafana-storage
```

## Loki structure

Docker VM internal storage:
```bash
/var/lib/docker/volumes/loki-data/_data/
├─ index/
├─ cache/
├─ chunks/
└─ wal/

```
