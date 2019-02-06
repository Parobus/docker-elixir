FROM elixir:1.7.4

# Note updating this forces a rebuild of all underlying containers.
ENV REFRESHED_AT=2018-11-23

RUN apt-get update && apt-get upgrade -y

RUN curl https://deb.nodesource.com/setup_11.x | bash -
RUN apt-get install -y nodejs

# Ensure node module bins can be found
ENV PATH=./node_modules/.bin:$PATH

CMD ["/bin/bash"]
