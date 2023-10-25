# FROM node:20 as build

# WORKDIR /usr/src/app

# COPY package.json .

# RUN npm install

# COPY . .

# CMD ["node", "index.js"]

# FROM build as main

# RUN npm install

# # COPY --from=build app/ /

# COPY --from=build . .

# # COPY . .

# EXPOSE 3000

# CMD ["node", "index.js"]

FROM mhart/alpine-node

WORKDIR /usr/src/app

COPY . .

RUN npm install

EXPOSE 3000

CMD ["node", "index.js"]



