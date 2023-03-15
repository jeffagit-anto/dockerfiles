# going to CI !
FROM debian:bullseye-slim

WORKDIR /

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
       texlive-xetex \
       texlive-fonts-extra\
       make

RUN groupadd -g 1001 xelatex && useradd --create-home --no-log-init -u 1001 -g 1001 xelatex

USER xelatex

WORKDIR /home/xelatex

CMD ["xelatex","--version"]
