FROM ubuntu:16.04

RUN apt-get update && apt-get install -y curl

COPY website.sh .

RUN chmod 741 website.sh

CMD ["/website.sh"]