# 🚀 Deploy Avanzato

Ora che hai guadagnato la fiducia dei pinguini, puoi procedere.

## 🐳 Creare un Dockerfile

```Dockerfile
FROM alpine:latest

RUN apk add --no-cache python3

CMD ["python3", "-m", "http.server", "8000"]
```

⚠️ Il pinguino anziano disapprova `latest`, ma oggi chiuderà un occhio.

## 🏗️ Build dell'immagine

```bash
docker build -t penguin-app .
```

## ▶️ Avvio del container

```bash
docker run -d -p 8000:8000 penguin-app
```

Ora il servizio è attivo su:

```
http://localhost:8000
```

## 🧊 Docker Compose (Livello Pinguino Imperiale)

```yaml
version: '3'

services:
  web:
    build: .
    ports:
      - "8000:8000"
```

Avvio:

```bash
docker-compose up -d
```

## 🐧 Conclusione

Se tutto funziona:

* i pinguini festeggiano
* tu hai deployato correttamente

Se non funziona:

* controlla i log
* e preparati al loro giudizio silenzioso
