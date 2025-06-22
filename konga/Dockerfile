# Datei: Dockerfile.konga
FROM pantsel/konga:latest
EXPOSE 1337
RUN npm install pg@latest sails-postgresql@latest
HEALTHCHECK CMD curl --fail http://localhost:1337 || exit 1
