ARG ES_VERSION

# Pulling metricbeat image
FROM docker.elastic.co/beats/metricbeat:${ES_VERSION}

# Copy metricbeat configuration
COPY config/metricbeat.yml /usr/share/metricbeat/metricbeat.yml

USER root
RUN chown root:metricbeat /usr/share/metricbeat/metricbeat.yml && chmod go-w /usr/share/metricbeat/metricbeat.yml
