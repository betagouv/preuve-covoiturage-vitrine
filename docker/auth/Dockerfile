FROM node:14
RUN wget -O /tmp/master.zip https://github.com/vencax/netlify-cms-github-oauth-provider/archive/refs/heads/master.zip
RUN mkdir -p /code
RUN unzip /tmp/master.zip -d /code
RUN cd /code/netlify-cms-github-oauth-provider-master && npm install
WORKDIR /code/netlify-cms-github-oauth-provider-master
ENV NODE_ENV=production
CMD npm start