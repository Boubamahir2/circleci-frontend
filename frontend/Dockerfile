FROM node

WORKDIR /app

COPY package.json ./

# RUN npm install --legacy-peer-deps
RUN npm install 

# RUN npm install --legacy-peer-deps

COPY . .

ENV REACT_APP_BASE_URL=http://localhost:5000/api/v1

EXPOSE 3000

CMD [ "npm", "start" ]




# FROM node:14-slim

# WORKDIR /usr/src/app

# COPY ./package.json ./
# COPY ./yarn.lock ./

# RUN yarn install

# COPY . .

# ENV REACT_APP_BASE_URL=http://localhost:5000/api

# EXPOSE 3000

# CMD [ "yarn", "start" ]



# ### First Stage ###
# FROM node

# WORKDIR /app

# COPY ./package.json ./
# COPY ./yarn.lock ./

# RUN yarn install

# COPY . .

# ARG BASE_URL
# ENV REACT_APP_BASE_URL=${BASE_URL}

# RUN yarn build

# ### Second Stage ###
# FROM caddy:2.1.1

# ARG CADDYFILE
# COPY ${CADDYFILE} /etc/caddy/Caddyfile

# COPY --from=builder /app/build/ /srv

# EXPOSE 3000
>>>>>>> 26aef91e3e13f9be78172c88c071743a536ef44e
