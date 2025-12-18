# Dockerize Node.js Application

## Projektübersicht

Dieses Projekt demonstriert das Dockerizing einer Node.js-Anwendung.

## Technologien

* Docker
* Node.js

## Projektbeschreibung

* Schreiben eines `Dockerfile`, um ein Docker-Image der Node.js-Anwendung zu bauen.
* Ausführen der Node.js-Anwendung innerhalb eines Docker-Containers.
* Das Repository enthält nur die notwendigen Dateien zum Docker-Build der App.

## Struktur

```
Dockerfile
README.md
app/               # Quellcode der Node.js App
package.json
package-lock.json
```

## Aufbau & Ausführung

1. Docker-Image bauen:

```bash
docker build -t nodejs-app .
```

2. Container starten:

```bash
docker run -d -p 3000:3000 nodejs-app
```

3. Anwendung ist erreichbar unter `http://localhost:3000`

## Hinweise

* Es wird nur das Node.js-Projekt dockerized, keine Datenbankverbindungen.
* Alles Wesentliche für die Prüfungsdemonstration befindet sich im Repo.

