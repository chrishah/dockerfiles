FROM ubuntu:18.04
MAINTAINER <philipp.resl@uni-graz.at>

RUN apt-get update && \
	apt-get install -y python3-pip python3
RUN apt-get install -y git parallel


RUN pip3 install numpy==1.14.0 scipy==1.0.0 six==1.11.0 Theano==1.0.1 git+https://github.com/Lasagne/Lasagne.git#egg=Lasagne-0.2.dev1

RUN mkdir /external

ENV PATH="/external:$PATH"
WORKDIR /data
CMD ["deeploc", "-h"]