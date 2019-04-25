FROM node
COPY . /app/
WORKDIR /app/web
RUN npm i && npm run build
CMD node ./lib/js/src/web.bs.js