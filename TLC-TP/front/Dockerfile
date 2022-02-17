
FROM node:14 as build
RUN git clone https://github.com/StefanLocke/doodlestudent.git
WORKDIR /doodlestudent/front

RUN npm install
RUN npm run build

FROM bunkerity/bunkerized-nginx as nginx
COPY --from=build /doodlestudent/front/dist/tlcfront /www
EXPOSE 80


