FROM elasticsearch:7.8.1
RUN yes | ./bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v7.8.1/elasticsearch-analysis-ik-7.8.1.zip
RUN mkdir -p ./config/analysis && chown -R elasticsearch:root ./config/analysis
COPY --chown=elasticsearch:root synonym.txt /usr/share/elasticsearch/config/analysis/