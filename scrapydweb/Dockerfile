FROM python:3

ENV USERNAME=admin
ENV PASSWORD=password
ENV SCRAPYD_HOST=127.0.0.1
ENV SCRAPYD_PORT=6800


ADD . /app

WORKDIR /app

#设置时区
RUN /bin/cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai' >/etc/timezone

RUN pip install --no-cache-dir -i https://mirrors.aliyun.com/pypi/simple/ scrapydweb

EXPOSE 5000

CMD [ "scrapydweb" ]
