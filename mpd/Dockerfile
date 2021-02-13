FROM arm64v8/alpine:latest
MAINTAINER J.S. Hoekstra

RUN set -xe && apk add --no-cache mpd mpc && setcap -r /usr/bin/mpd
VOLUME /var/lib/mpd
EXPOSE 6600
CMD ["mpd", "--stdout", "--no-daemon"]
