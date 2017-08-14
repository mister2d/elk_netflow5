# This will prepare a logstash with netflow supported.
# The logstash can be started with `logstash agent -f /etc/logstash/conf.d/`, which will use the logstash_netflow.conf as the configuration file.

FROM logstash:5.5.1
MAINTAINER drdukes@gmail.com

ENV DEBIAN_FRONTEND noninteractive

COPY logstash_netflow5.conf /etc/logstash/conf.d/
COPY logstash_syslog.conf /etc/logstash/conf.d/

RUN /usr/share/logstash/bin/logstash-plugin install --no-verify logstash-codec-netflow
