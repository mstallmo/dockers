FROM rust:1.34.1

RUN apt-get -y -qq update

# Install Node.JS
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install nodejs -y

# Install aws-cli
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN python get-pip.py
RUN pip install awscli --upgrade
