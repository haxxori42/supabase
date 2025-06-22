# Datei: Dockerfile.konga
FROM pantsel/konga:latest
EXPOSE 1337
HEALTHCHECK CMD curl --fail http://localhost:1337 || exit 1
