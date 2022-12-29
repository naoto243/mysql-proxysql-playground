ARG PROXYSQL_VERSION="2.0.12"
FROM proxysql/proxysql:${PROXYSQL_VERSION}

RUN export GIT_SSL_NO_VERIFY=1

RUN mv /etc/apt/sources.list.d /etc/apt/sources.list.d.back
RUN apt-get install -y ca-certificates
RUN apt-get update && apt-get install -y \
    mysql-client \
    gettext-base \
 && rm -rf /var/lib/apt/lists/*
