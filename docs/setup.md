# 🧊 Setup dell'Ambiente

Prima di iniziare il deploy, i pinguini richiedono un ambiente adeguato.

## 🐧 Requisiti

* Docker installato
* Accesso alla CLI
* Rispetto per il ghiaccio

## 🔧 Installazione Docker

```bash
sudo apt update
sudo apt install docker.io
```

Verifica:

```bash
docker --version
```

Se il comando funziona, il pinguino annuisce.

## 📦 Primo Container

```bash
docker run hello-world
```

Se appare un messaggio di successo:

> Il pinguino capo ti osserva approvando lentamente.

## 🧠 Best Practice

* Usa immagini leggere (alpine > balena gigante)
* Evita di runnare tutto come root
* Nomina i container con dignità

Prossimo passo: imparare il deploy serio.
