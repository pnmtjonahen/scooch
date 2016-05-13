FROM node
MAINTAINER IvoNet <webmaster@ivonet.nl>
ENV VERSION 0.0.2
RUN git clone -b $VERSION --single-branch https://github.com/IvoNet/scooch.git
WORKDIR /scooch
RUN npm install && ln -s /scooch/slides /slides && ln -s /scooch/templates /templates && ln -s /scooch/themes /themes
EXPOSE 3000
VOLUME /slides
VOLUME /templates
VOLUME /themes
ENTRYPOINT npm start