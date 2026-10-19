FROM postgres:16

RUN apt-get update \
    && apt-get install -y --no-install-recommends pgbackrest \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir -p /var/lib/pgbackrest \
    && chown postgres:postgres /var/lib/pgbackrest \
    && chmod 750 /var/lib/pgbackrest
