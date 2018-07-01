FROM jxzsxsp/ontology:1.0.0
ENV ONTOLOGY_PATH /data/ontology
ENV ACCOUNT_PASSWORD passwordtest
EXPOSE 20334 20335 20336 20337 20338 20339 20000
WORKDIR $ONTOLOGY_PATH
CMD ["/bin/sh", "-c", "echo $ACCOUNT_PASSWORD | ./ontology --testmode"]
