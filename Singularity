Bootstrap: docker
From: ubuntu:18.04

%labels
    Maintainer Belcour A.
    Version v1.3.1
    Description m2m Singularity recipe

%environment
     export PYTHONIOENCODING=utf8

%post
     apt-get -y update && \
     DEBIAN_FRONTEND=noninteractive apt-get install -y \
     curl \
     git \
     python3.6-dev \
     python3.6-distutils ;\
     apt-get clean ;\
     apt-get purge ;\
     curl https://bootstrap.pypa.io/get-pip.py | python3;\
     pip install padmet clyngor-with-clingo clyngor pandas pipdeptree==0.13.2;\
     pip install Metage2Metabo==1.3.1
