FROM python:alpine3.6

MAINTAINER song.jin

RUN apk update
RUN apk add --no-cache build-base
RUN pip install pandas

ADD . /app/

WORKDIR /app/

# anything after ADD will not be cached since Docker 0.7
# so it is good to include things in:
# "RUN pip install -r requirements.txt" to be flexible
