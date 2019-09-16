FROM elixir:1.9.1

# Note updating this forces a rebuild of all underlying containers.
ENV REFRESHED_AT=2019-09-16

RUN apt-get update && apt-get upgrade -y

RUN curl https://deb.nodesource.com/setup_11.x | bash -
RUN apt-get install -y nodejs

# Ensure node module bins can be found
ENV PATH=./node_modules/.bin:$PATH

CMD ["/bin/bash"]
