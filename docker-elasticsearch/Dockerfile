# This will prepare a elasticsearch with head, bigdesk plugins installed.
# See http://localhost:9200/_plugin/head/ and http://localhost:9200/_plugin/bigdesk/ after booted.
# A logstash_netflow- started index will be parsed according to the logstash_netflow.json.

FROM elasticsearch:5.5.1
MAINTAINER drdukes@gmail.com

#RUN apk add --update curl && \
#    rm -rf /var/cache/apk/*

#RUN chown -R elasticsearch: /usr/share/elasticsearch

COPY ./logstash_netflow5.json /tmp/
