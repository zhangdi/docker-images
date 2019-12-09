FROM python:3

ADD . /app

WORKDIR /app

COPY ./scrapyd.conf /etc/scrapyd/

COPY ./pip.conf ~/.pip/

RUN pip install --no-cache-dir -i https://mirrors.aliyun.com/pypi/simple/ scrapyd requests

EXPOSE 6800

CMD [ "scrapyd" ]
