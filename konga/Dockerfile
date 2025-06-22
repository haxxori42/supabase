# Datei: Dockerfile.konga
FROM pantsel/konga:latest
EXPOSE 1337
CMD ["node", "bin/konga.js"]
HEALTHCHECK CMD curl --fail http://localhost:1337 || exit 1
