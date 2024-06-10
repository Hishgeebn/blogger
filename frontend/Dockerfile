FROM node:18-alpine3.19

WORKDIR /blogger-frontend

ENV NEXT_TELEMETRY_DISABLED 1

COPY package.json .
RUN npm install

COPY . .

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host"]