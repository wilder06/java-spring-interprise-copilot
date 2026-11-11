# Java 25 — referencia de equipo

- Confirmar toolchain y compatibilidad de plugins antes de usar características nuevas.
- Preferir APIs estándar y características finalizadas.
- Evitar preview features salvo autorización.
- Virtual Threads son apropiados para workloads bloqueantes con alta concurrencia; no aceleran CPU-bound.
- Usar profiling/benchmarks representativos; no inferir mejoras solo por menor coste de hilo.
- Considerar pinning/monitoring y compatibilidad de librerías nativas/bloqueantes según JDK y runtime.
