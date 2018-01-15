FROM docker.elastic.co/elasticsearch/elasticsearch
RUN elasticsearch-plugin remove x-pack

# cleanup unused modules to slim image
RUN rm -rf modules/aggs-matrix-stats
RUN rm -rf modules/ingest-common
RUN rm -rf modules/lang-expression
RUN rm -rf modules/lang-groovy
RUN rm -rf modules/lang-mustache
RUN rm -rf modules/percolator
RUN rm -rf modules/transport-netty3
