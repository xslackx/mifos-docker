FROM mysql:5.5

RUN mkdir -p /docker-entrypoint-initdb.d 	&& cd / 

COPY ./00-create-databases.sql /docker-entrypoint-initdb.d/00-create-databases.sql

COPY ./01-mifospltaform-tenants-first-time-install.sql /docker-entrypoint-initdb.d/01-mifospltaform-tenants-first-time-install.sql

VOLUME /docker-entrypoint-initdb.d
