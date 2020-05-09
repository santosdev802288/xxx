FROM devopsfaith/krakend:1.1.1
USER root
RUN apt-get update && apt-get install vim -y && apt-get install nmap -y && apt-get install iputils-ping -y
COPY krakend.json /etc/krakend/krakend.json