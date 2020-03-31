FROM python:3.7
MAINTAINER Anirban Deb

COPY ./djangoModule /djangoModule
WORKDIR /djangoModule
RUN pip install -r requirements.txt && \
  pip install gunicorn

COPY ./dockerfile/entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
