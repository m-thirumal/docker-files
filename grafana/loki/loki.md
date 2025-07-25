# Centralized Loki

Alloy will collect logs from different server and send it to centralized loki.

``` shell
[ Server A: Alloy ] ─────┐
[ Server B: Alloy ] ───┬─┴──> [ Central Loki Server ]
[ Server C: Alloy ] ───┘
```