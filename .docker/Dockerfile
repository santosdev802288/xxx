FROM devopsfaith/krakend:1.1.1
USER root
RUN apt-get update && apt-get install vim -y && apt-get install nmap -y && apt-get install iputils-ping -y \
&& apt-get install procps -y && apt-get install net-tools -y
COPY krakend.json /etc/krakend/krakend.json