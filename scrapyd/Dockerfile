FROM python:3

ADD . /app

WORKDIR /app

COPY ./scrapyd.conf /etc/scrapyd/

COPY ./pip.conf ~/.pip/

#设置时区
RUN /bin/cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai' >/etc/timezone

RUN pip install --no-cache-dir -i https://mirrors.aliyun.com/pypi/simple/ scrapyd requests

EXPOSE 6800

CMD [ "scrapyd" ]
