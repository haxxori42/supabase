# Nutze stabile, vorkonfigurierte Kong-Version mit Luarocks + luaossl vorinstalliert
FROM kong:3.6

# Optional: Wenn du weiterhin eine kong.yml nutzen willst – ansonsten auskommentieren
# COPY ./kong.yml /home/kong/kong.yml

# Stelle sicher, dass korrekter User verwendet wird
USER kong
EXPOSE 8000 8443 8001 8002
# Starte im typischen DB-Modus (Admin API erreichbar unter :8001)

# Führt Migration **vor** dem eigentlichen Start durch
ENTRYPOINT ["/docker-entrypoint.sh", "kong", "docker-start"]

