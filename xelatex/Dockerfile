# going to CI !
FROM debian:bullseye-slim

WORKDIR /

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
       texlive-latex-extra \
       texlive-xetex \
       texlive-fonts-extra

RUN groupadd -r xelatex && useradd --no-log-init -r -g xelatex xelatex

USER xelatex

WORKDIR /home/xelatex

CMD ["xelatex","--version"]
