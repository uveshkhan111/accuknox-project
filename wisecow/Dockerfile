FROM ubuntu:22.04

RUN apt-get update && \
    apt-get install -y cowsay fortune netcat bash && \
    apt-get clean


ENV PATH="/usr/games:${PATH}"

WORKDIR /wisecow

COPY wisecow.sh .

RUN chmod +x wisecow.sh

EXPOSE 4499

CMD ["bash", "wisecow.sh"]