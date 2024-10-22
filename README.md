# Pterodactyl-Docker-Images

## Übersicht

Dieses Projekt enthält Docker-Images für die Verwendung mit Pterodactyl. Es umfasst verschiedene Versionen von Java und stellt sicher, dass die Images auf verschiedenen Plattformen wie `linux/amd64` und `linux/arm64` funktionieren.

## Verzeichnisstruktur

- `.github/workflows/Java.yml`: GitHub Actions Workflow zum Erstellen und Veröffentlichen der Docker-Images.
- `java/entrypoint.sh`: Entrypoint-Skript, das beim Starten des Containers ausgeführt wird.
- `java/21/Dockerfile`: Dockerfile für Java 21.

## Docker-Images

Die Docker-Images werden automatisch erstellt und in die GitHub Container Registry (`ghcr.io`) gepusht. Die Tags der Images folgen dem Schema `java_<version>`.

## Verwendung

### Docker-Image ausführen

Um ein Docker-Image auszuführen, verwenden Sie den folgenden Befehl:

```sh
docker run -it ghcr.io/coho04/pterodactyl-docker-images:java_<version># Pterodactyl-Docker-Images