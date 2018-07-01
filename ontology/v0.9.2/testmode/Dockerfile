FROM jxzsxsp/ontology
ENV ONTOLOGY_PATH /var/ontology
ENV ACCOUNT_PASSWORD passwordtest
EXPOSE 20334 20335 20336 20337 20338 20339
WORKDIR $ONTOLOGY_PATH
CMD ["/bin/sh", "-c", "echo $ACCOUNT_PASSWORD | ./ontology --testmode -w data/wallet.dat"]
