## Modulo 2: Containers, Networking, Web server, TLS (4h)

### Docker intro (30’)

- **Concetti:** Container, Image, Volume, Network
- **Tools:** `docker run`, `docker exec`, `docker ps`, `docker images`
- **Esercizio:** 
  - docker run hello-world

---

### Docker compose intro (30’)

- **Concetti:** Compose, Network, Volume
- **Tools:** `docker compose up`, `docker compose down`, `docker compose ps`, `docker compose logs`
- **Esercizio:** 
  - Creare container con volume
  - Montare volume
  - Analisi log

---

### Networking Fundamentals (30’)

- **Concetti:** IP, subnet, gateway, DNS, `/etc/hosts`
- **Tools:** `ping`, `traceroute`, `nslookup/dig`, `ss/netstat`
- **Sicurezza:** Firewall, WAF, porte TCP/UDP
- **Esercizio:** Configurare Network tra container

---

### Traefik e NGINX (30’)

- **Ruoli:** Static server vs Reverse proxy
- **Esercizio:** 
  - Usare Traefik come reverse proxy
  - Servire pagina statica
  - Analisi log access/error

---

### SSL/TLS Basics (30’)

- **Componenti:** Certificati, Chiavi, CA, CSR
- **Pratica:**
  - Generare self-signed cert (OpenSSL)
  - Configurare HTTPS su Traefik (8443)
  - Test `curl -k`

---

### JSON, YAML, JSONPath (20’)

- **Formati:** Sintassi e differenze
- **Tools:** `jq`, `yq`
- **Esercizio:**
  - Parsing JSON con `jq`
  - Conversione YAML/JSON

---

### Checkpoint (10’)

- Quiz e Retrospettiva
