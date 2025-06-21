# Nutze stabile, vorkonfigurierte Kong-Version mit Luarocks + luaossl vorinstalliert
FROM kong/kong-gateway:3.5.0.0-alpine

# Optional: Wenn du weiterhin eine kong.yml nutzen willst – ansonsten auskommentieren
# COPY ./kong.yml /home/kong/kong.yml

# Stelle sicher, dass korrekter User verwendet wird
USER kong

# Starte im typischen DB-Modus (Admin API erreichbar unter :8001)
ENTRYPOINT ["/docker-entrypoint.sh", "kong", "docker-start"]
