FROM python:alpine3.11
ENTRYPOINT ["gallery-dl"]
CMD ["--help"]

COPY . /opt/gallery-dl

RUN apk add --update --no-cache ffmpeg && \
    pip install --upgrade --no-cache-dir youtube_dl && \
    pip3 install -e /opt/gallery-dl