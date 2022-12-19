FROM node:alpine
USER node
WORKDIR "/app"
COPY ./package.json ./
RUN npm install
COPY . .
COPY --chown=node:node ./ ./
CMD ["npm", "run", "start"]