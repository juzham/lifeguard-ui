FROM ruby:2.6.5

# Getting Yarn Installed...
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN apt update && apt install -y yarn

RUN apt-get update -qq && apt-get install -y nodejs postgresql-client

# Include "shush" to decode KMS_ENCRYPTED_STUFF
RUN curl -sL -o /usr/local/bin/shush \
  https://github.com/realestate-com-au/shush/releases/download/v1.3.4/shush_linux_amd64 \
  && chmod +x /usr/local/bin/shush
