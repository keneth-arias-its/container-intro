## Modulo 2: Networking, Web server, TLS (4h)

---

### Networking Fundamentals (60’)

- **Concetti:** IP, subnet, gateway, DNS, `/etc/hosts`
- **Tools:** `ping`, `traceroute`, `nslookup/dig`, `ss/netstat`
- **Sicurezza:** Firewall `ufw`, porte TCP/UDP
- **Esercizio:** Configurare NIC Host-only e firewall

---

### NGINX e Caddy (30’)

- **Ruoli:** Static server vs Reverse proxy
- **Esercizio:** 
  - Installare NGINX
  - Servire pagina statica
  - Analisi log access/error

---

### Gunicorn e Uvicorn (30’)

- **Concetti:** Web Server vs App Server
- **Protocolli:** WSGI (Sync) vs ASGI (Async)
- **Gunicorn:**
  - WSGI (Flask/Django)
  - Worker & Forking
- **Uvicorn:**
  - ASGI (FastAPI)
  - Performance async
- **Esercizio:** Eseguire app con Gunicorn/Uvicorn

---

### SSL/TLS Basics (40’)

- **Componenti:** Certificati, Chiavi, CA, CSR
- **Pratica:**
  - Generare self-signed cert (OpenSSL)
  - Configurare HTTPS su NGINX (8443)
  - Test `curl -k`

---

### JSON, YAML, JSONPath (40’)

- **Formati:** Sintassi e differenze
- **Tools:** `jq`, `yq`
- **Esercizio:**
  - Parsing JSON con `jq`
  - Conversione YAML/JSON

---

### Checkpoint (10’)

- Quiz e Retrospettiva
