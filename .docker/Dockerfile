FROM devopsfaith/krakend:1.1.1

WORKDIR /app

COPY ./partials ./partials
# COPY ./settings ./settings
# COPY ./templates ./templates

ENV FC_ENABLE=1
ENV FC_PARTIALS="/app/partials"
# ENV FC_SETTINGS="/app/settings"
# ENV FC_TEMPLATES="/app/templates"
# ENV FC_OUT="/app/out.json" 

USER root

ENV COMPlus_EnableDiagnostics=0

RUN apt-get update
RUN apt-get install vim -y
RUN apt-get install nmap -y
RUN apt-get install iputils-ping -y
RUN apt-get install procps -y
RUN apt-get install net-tools -y

RUN adduser --disabled-password --gecos "" app -u 1000

USER 1000

COPY krakend.json /etc/krakend/krakend.json