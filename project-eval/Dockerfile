FROM node:10 as build-deps
WORKDIR /usr/src/app
ARG git_repo=--help
ENV CI=true
RUN git clone ${git_repo} /usr/src/app
RUN npm i
ENTRYPOINT npm run testonce