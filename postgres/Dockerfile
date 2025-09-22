FROM postgres:15

# Instalar locales y generar es_MX.UTF-8
RUN apt-get update && apt-get install -y locales \
    && sed -i '/es_MX.UTF-8/s/^# //g' /etc/locale.gen \
    && locale-gen es_MX.UTF-8 \
    && update-locale LANG=es_MX.UTF-8

# Variables de entorno para Postgres
ENV LANG=es_MX.UTF-8
ENV LC_COLLATE=es_MX.UTF-8
ENV LC_CTYPE=es_MX.UTF-8
ENV LC_ALL=es_MX.UTF-8
