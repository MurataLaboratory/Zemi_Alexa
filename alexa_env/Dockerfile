From ubuntu:latest

ENV DEBIAN_FRONTEND=noninteractive

RUN echo "building"

RUN apt-get update && apt-get install -y \
vim \
git \
make \
build-essential \
libssl-dev \
zlib1g-dev \
libbz2-dev \
libreadline-dev \
libsqlite3-dev \
libncurses5-dev \
libncursesw5-dev \
xz-utils \
tk-dev \
libffi-dev \
liblzma-dev \
openssl \
python3-dev \
&& apt-get install -y locales curl python3-distutils \
&& curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py \
&& python3 get-pip.py \
&& pip install -U pip \
&& mkdir /code \
&& cd code \
&& git clone https://github.com/MurataLaboratory/Zemi_Alexa.git

RUN echo "library installed !! "

WORKDIR code
ADD requirement.txt /code
RUN pip install -r requirement.txt


