# build environment
FROM node:9.6.1
#  NODE_ENV: production
WORKDIR /usr/src
ENV PATH /usr/src/app/node_modules/.bin:$PATH
COPY . /usr/src/
RUN rm -rf /usr/src/node_modules
RUN npm install
RUN npm install -g swagger
# install aws cli
# install git
EXPOSE 10010
CMD ["swagger", "project", "start", "-m"]