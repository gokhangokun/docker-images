FROM docker.elastic.co/logstash/logstash:5.6.3
RUN logstash-plugin install logstash-filter-drop
RUN rm -f /usr/share/logstash/pipeline/logstash.conf
ADD config/ /usr/share/logstash/pipeline/
ADD config/ /usr/share/logstash/config/
RUN logstash-plugin remove x-pack
RUN sed -i '/xpack/d' /usr/share/logstash/config/logstash.yml