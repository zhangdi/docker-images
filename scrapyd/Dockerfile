FROM python:3

ADD . /app

WORKDIR /app

COPY ./scrapyd.conf /etc/scrapyd/

COPY ./pip.conf ~/.pip/pip.conf

RUN pip install --no-cache-dir scrapyd

EXPOSE 6800

CMD [ "scrapyd" ]