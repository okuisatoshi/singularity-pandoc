Bootstrap:docker
From: ubuntu:18.04

%post
apt-get update && \
apt-get install -y build-essential git curl wget &&\
apt-get install -y tzdata language-pack-ja &&\
apt-get install -y texlive-base texlive-lang-japanese texlive-luatex latexmk xzdec pandoc &&\
apt-get clean
update-locale LANG=ja_JP.UTF8
dpkg-reconfigure tzdata

%runscript
pandoc "$@"



