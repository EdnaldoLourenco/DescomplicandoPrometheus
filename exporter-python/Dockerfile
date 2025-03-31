FROM python:3.12-slim

LABEL maintainer Ednaldo Lourenço <ednaldolourencojr@gmail.com>
LABEL description "Dockerfile do primeiro exporter"

WORKDIR /app
COPY . /app
RUN pip3 install -r requirements.txt

CMD python3 exporter.py
