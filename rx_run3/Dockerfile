FROM    cern/alma9-base:latest
WORKDIR /opt/rx_run3 
COPY    requirements.txt .
RUN     dnf install -y epel-release             &&\ 
        dnf install -y root python3 python3-pip &&\
        dnf install -y xrootd-client xrootd-server python3-xrootd && \
        python3 -m pip install --upgrade pip && \
        python3 -m pip install --no-cache-dir -r requirements.txt
