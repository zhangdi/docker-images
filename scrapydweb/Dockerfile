FROM python:3

ENV USERNAME=admin
ENV PASSWORD=password


ADD . /app

WORKDIR /app

COPY ./pip.conf ~/.pip/

RUN pip install --no-cache-dir scrapydweb

EXPOSE 5000

CMD [ "scrapydweb" ]