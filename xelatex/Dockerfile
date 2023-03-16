# going to CI !!
FROM debian:bullseye-slim

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
       texlive-xetex \
       texlive-fonts-extra\
       texlive-latex-extra

CMD ["xelatex","--version"]
