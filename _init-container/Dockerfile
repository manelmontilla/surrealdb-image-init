FROM surrealdb/surrealdb:v2.0.0-alpha.6 AS surrealdb
FROM   ubuntu:20.04
COPY --from=surrealdb /surreal /surreal
RUN apt-get update && apt-get install -y curl
CMD [ "/bin/sh" ]
