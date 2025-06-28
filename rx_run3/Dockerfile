FROM    cern/alma9-base:latest
WORKDIR /opt/rx_run3 
COPY    requirements.txt .
RUN     dnf install -y epel-release             &&\ 
        dnf install -y python312 python3.12-pip &&\
        dnf install -y root xrootd-client xrootd-server python3-xrootd && \
        python3.12 -m pip install --upgrade pip && \
        python3.12 -m pip install --no-cache-dir -r requirements.txt
RUN     echo "alias python=python3" >> /etc/bash.bashrc
