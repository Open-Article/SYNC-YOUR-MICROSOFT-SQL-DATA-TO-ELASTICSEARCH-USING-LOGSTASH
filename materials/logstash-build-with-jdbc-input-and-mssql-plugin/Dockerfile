FROM docker.elastic.co/logstash/logstash:7.3.1

RUN logstash-plugin install logstash-filter-jdbc_streaming
RUN logstash-plugin install logstash-filter-aggregate
RUN logstash-plugin install logstash-input-jdbc
RUN logstash-plugin install logstash-filter-translate

COPY ./jars /usr/share/logstash/logstash-core/lib/jars
