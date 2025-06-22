# Datei: Dockerfile.konga
FROM pantsel/konga:latest
EXPOSE 1337
RUN npm install sails-postgresql@0.11.0 pg@7.18.2
HEALTHCHECK CMD curl --fail http://localhost:1337 || exit 1
