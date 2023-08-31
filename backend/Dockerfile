## Build
# docker build -t backend:0.1.0 .
## Run
# docker run backend:0.1.0

FROM oraclelinux:8.8

# Install Oracle Client (oracle's libs)
RUN dnf install oracle-instantclient-release-el8 -y
RUN dnf install oracle-instantclient-basic -y

# Install Nodejs
RUN dnf module enable nodejs:16 -y
RUN dnf module install nodejs -y

COPY . /opt/app

WORKDIR /opt/app

CMD ["npm", "start"]
