# Docker image that contains a Spring Boot application.
# Base image - use alpine, a minimalistic Linux release, to conserve space
FROM docker-registry.ontotext.com/graphdb-ee:sava

# Init with the soaas repository configuration.
COPY config.ttl /opt/graphdb/dist/data/repositories/soaas/config.ttl
COPY graphdb.license /opt/graphdb/dist/conf/graphdb.license

ENTRYPOINT ["/opt/graphdb/dist/bin/graphdb"]

EXPOSE 7200
