FROM ubuntu:latest
RUN apt-get update
RUN apt-get install -y wget git firefox nodejs nodejs-legacy npm
RUN apt-get install -y build-essential mysql-server libmysqld-dev bzip2 libjpeg$
RUN apt-get install -y pike7.8 pike7.8-bzip2 pike7.8-svg
RUN apt-get install -y libxml2-dev libxslt1-dev automake flex
RUN npm install -g npm bower gulp coffee-script jasmine-node frisby
RUN cd home
RUN wget -c https://raw.githubusercontent.com/societyserver/sTeam/steam-package$
RUN git clone www.github.com/societyserver/steam.git
RUN cd sTeam
RUN git checkout societyserver-source
RUN ./build
RUN sudo ./install
RUN cd ..
RUN git clone https://github.com/societyserver/sTeam-web-interface-gsoc-2015.git
RUN cd sTeam-web-interface-gsoc-2015
RUN npm install
RUN cd ..
RUN git clone https://github.com/societyserver/steam-rest.git
RUN cd steam-rest
RUN npm install
RUN cd ..



