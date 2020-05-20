FROM ubuntu:18.04

# RUN export DEBIAN_FRONTEND=noninteractive
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get -yqq update           
RUN apt-get install -yqq apt-utils
RUN apt-get install -yqq tzdata    
RUN apt-get install -yqq git       
RUN apt-get install -yqq awscli    
RUN apt-get install -yqq vim      
RUN apt-get install -yqq php       

# Laravel requirement
RUN apt-get install -yqq php-common php-bcmath php-ctype php-json php-mbstring php-tokenizer php-xml
RUN apt-get install -yqq composer 
RUN apt-get install -yqq unzip  
RUN apt-get install -yqq wget  

# Packer
RUN wget https://releases.hashicorp.com/packer/1.5.1/packer_1.5.1_linux_amd64.zip -q 
RUN unzip packer_1.5.1_linux_amd64.zip -d /usr/bin/ && rm packer_1.5.1_linux_amd64.zip

CMD [ "/bin/bash" ]