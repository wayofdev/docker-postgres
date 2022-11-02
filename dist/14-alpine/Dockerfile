# Auto-generated via Ansible: edit src/Dockerfiles/all/Dockerfile.j2 instead.

FROM postgres:14

# Labels
# https://github.com/opencontainers/image-spec/blob/main/annotations.md
LABEL "maintainer"="lotyp <lotyp7@gmail.com>"
LABEL "vendor"="wayofdev"
LABEL "org.opencontainers.image.authors"="lotyp <lotyp7@gmail.com>"
LABEL "org.opencontainers.image.url"="https://hub.docker.com/r/wayofdev/postgres"
LABEL "org.opencontainers.image.documentation"="https://github.com/wayofdev/docker-postgres"
LABEL "org.opencontainers.image.source"="https://github.com/wayofdev/docker-postgres"
LABEL "org.opencontainers.image.vendor"="wayofdev"
LABEL "org.opencontainers.image.licenses"="MIT"
LABEL "org.opencontainers.image.ref.name"="14-alpine"
LABEL "org.opencontainers.image.title"="postgres-14-alpine"
LABEL "org.opencontainers.image.description"="postgres-14-alpine"

# https://vsupalov.com/docker-env-vars/
ARG POSTGRES_PASSWORD=postgres
ENV POSTGRES_PASSWORD=${POSTGRES_PASSWORD}

COPY configs/enable-extensions.sql /docker-entrypoint-initdb.d
