FROM debian:stretch

# Note updating this forces a rebuild of all underlying containers.
ENV REFRESHED_AT=2019-09-20

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y curl locales

# Set the locale
RUN sed -i -e 's/# en_GB.UTF-8 UTF-8/en_GB.UTF-8 UTF-8/' /etc/locale.gen && \
    locale-gen

ENV LANG en_GB.UTF-8
ENV LANGUAGE en_GB:en
ENV LC_ALL en_GB.UTF-8

CMD ["/bin/bash"]
