FROM circleci/node:8-stretch

# Install heroku cli
RUN sudo wget https://cli-assets.heroku.com/branches/stable/heroku-linux-amd64.tar.gz \
    && sudo mkdir -p /usr/local/lib /usr/local/bin \
    && sudo tar -xzf heroku-linux-amd64.tar.gz -C /usr/local/lib \
    && sudo ln -s /usr/local/lib/heroku/bin/heroku /usr/local/bin/heroku \
    && sudo rm heroku-linux-amd64.tar.gz

# Install bower
RUN yarn add global bower ember-cli
