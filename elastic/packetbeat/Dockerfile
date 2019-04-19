ARG ES_VERSION

# Pulling packet image
FROM docker.elastic.co/beats/packetbeat:${ES_VERSION}
COPY config/packetbeat.yml /usr/share/packetbeat/packetbeat.yml
USER root
RUN chown root:packetbeat /usr/share/packetbeat/packetbeat.yml && chmod go-w /usr/share/packetbeat/packetbeat.yml