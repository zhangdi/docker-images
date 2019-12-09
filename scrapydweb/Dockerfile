FROM python:3

ENV USERNAME=admin
ENV PASSWORD=password


ADD . /app

WORKDIR /app

RUN pip install --no-cache-dir -i https://mirrors.aliyun.com/pypi/simple/ scrapydweb

EXPOSE 5000

CMD [ "scrapydweb" ]