FROM docker.elastic.co/kibana/kibana:5.6.3
RUN bin/kibana-plugin remove x-pack
ADD config/ /usr/share/kibana/config/
