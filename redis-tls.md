# Redis TLS — checklist

- Cliente y versión: completar según proyecto.
- TLS: CA/truststore, hostname verification y protocolo.
- ACL: usuario y secreto desde gestor de secretos.
- Timeouts: conexión, comando y lectura.
- Pool: dimensionar según cliente y concurrencia; evitar pools duplicados.
- Cache: TTL, serialización, invalidación y fallback.
- GCP Memorystore: verificar modo de conexión, red, TLS y certificados según instancia/versión.
- Local: reproducir TLS cuando sea viable; no relajar producción para simplificar local.
