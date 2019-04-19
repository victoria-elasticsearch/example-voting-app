ARG ES_VERSION

FROM docker.elastic.co/beats/heartbeat:${ES_VERSION}
COPY config/heartbeat.yml /usr/share/heartbeat/heartbeat.yml
USER root
RUN chown root:heartbeat /usr/share/heartbeat/heartbeat.yml  && chmod go-w /usr/share/heartbeat/heartbeat.yml
