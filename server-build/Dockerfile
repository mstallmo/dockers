FROM rust:1.34.1

RUN apt-get -y -qq update
RUN apt-get install curl -y
RUN apt-get -y -qq install python-dev

# Install Node.JS
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install nodejs -y

# Install aws-cli
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN python get-pip.py
RUN pip install awscli --upgrade

# Install heroku-cli
RUN curl https://cli-assets.heroku.com/install-ubuntu.sh | sh
