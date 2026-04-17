# 🚀 High-Performance VPS Infrastructure

Este repositorio contiene la configuración de infraestructura para un entorno de alto rendimiento, optimizado para exprimir al máximo un VPS de **16GB RAM y 4 vCPUs** (Hetzner/Oracle Cloud).

## 🛠️ Stack Tecnológico

- **Base de Datos:** PostgreSQL 18.3 (Custom Tuning)
- **Caché:** Redis 8.6 (LRU Policy)
- **Storage:** RustFS (High Efficiency I/O)
- **Arquitectura:** Docker Compose con límites de recursos y red interna.

---

## ⚙️ Configuración (.env)

Copia este bloque en un archivo llamado `.env` en la raíz del proyecto:

```env
# --- PostgreSQL ---
DB_POSTGRES_PORT=5432
DB_POSTGRES_USER=admin
DB_POSTGRES_PASSWORD=tu_password_seguro

# --- Redis ---
DB_REDIS_PORT=6379

# --- RustFS Storage ---
STORAGE_ACCESS_PORT=20000
STORAGE_ACCESS_KEY=tu_access_key
STORAGE_SECRET_KEY=tu_secret_key
```
