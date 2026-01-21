# Container Intro - Setup (Docker Edition)

## 🎓 Compito / Assignment

**Obiettivo**: Eseguire l'ambiente di laboratorio basato su Docker e dimostrarne il funzionamento.

1.  Segui la guida qui sotto per avviare lo stack con Docker Compose.
2.  Verifica che il server Minecraft e la mappa Dynmap siano accessibili.
3.  Carica in questo repository gli **Screenshot** richiesti (come quelli in `screenshots/`).

---

Questo repository contiene la configurazione **Docker Compose** per avviare un server Minecraft con il plugin Dynmap integrato.

## 1. Prerequisiti

Assicurati di avere installato:
*   **Docker Desktop**
*   **Git**

## 2. Scaricare il Repository

Clona il repository (se non l'hai già fatto):

```powershell
git clone https://github.com/keneth-arias-its/container-intro.git
cd container-intro
```

## 3. Avvio ambiente (Docker Compose)

Per avviare il server Minecraft e Dynmap, esegui il seguente comando nella cartella del progetto:

```powershell
docker compose up -d
```

Questo scaricherà l'immagine del server e avvierà il container `mc`.

### Verificare lo stato
Puoi controllare i log per vedere quando il server è pronto:

```powershell
docker compose logs -f mc
```

Premi `Ctrl+C` per uscire dai log.

## 4. Accesso alle Applicazioni

Una volta avviato, i servizi sono accessibili ai seguenti indirizzi:

### 🎮 Minecraft Server
*   **Indirizzo Server**: `localhost:25565`
*   **Versione**: 1.21.1
*   Collegati usando il tuo client Minecraft oppure [UltimMC](https://ultimmc.com/download-ultimmc-launcher/).

### 🗺️ Dynmap (Mappa Web)
*   **URL**: [http://localhost:8123](http://localhost:8123)
*   Visualizza la mappa del mondo di gioco in tempo reale direttamente dal browser.

## 5. Dimostrazione (Screenshots)

Ecco come appare l'ambiente funzionante:

### Dynmap Webpage
![Dynmap](screenshots/dynmap.png)

### Minecraft Server Status
![Server Status](screenshots/MC.png)

## 6. Spegnimento

Per fermare e rimuovere i container:

```powershell
docker compose down
```

I dati del mondo di gioco sono salvati nel volume Docker `data`, quindi non verranno persi al riavvio.

---
## Licenza
Distribuito sotto licenza MIT.