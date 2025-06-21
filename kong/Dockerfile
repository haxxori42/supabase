# Nutze stabile, vorkonfigurierte Kong-Version mit Luarocks + luaossl vorinstalliert
FROM kong:3.5

# Optional: Wenn du weiterhin eine kong.yml nutzen willst – ansonsten auskommentieren
# COPY ./kong.yml /home/kong/kong.yml

# Stelle sicher, dass korrekter User verwendet wird
USER kong
EXPOSE 8000 8443
# Starte im typischen DB-Modus (Admin API erreichbar unter :8001)
ENTRYPOINT ["/docker-entrypoint.sh", "kong", "docker-start"]

#ENTRYPOINT ["/bin/sh", "-c", "kong migrations bootstrap && /docker-entrypoint.sh kong docker-start"]
