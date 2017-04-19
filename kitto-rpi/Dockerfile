FROM resin/raspberry-pi2-node

RUN apt-get update
RUN apt-get install apt-transport-https
RUN echo 'deb https://packages.erlang-solutions.com/debian jessie contrib' > /etc/apt/sources.list.d/erlang.list
RUN apt-get update
RUN apt-get install -y erlang xz-utils git make elixir
RUN mix local.hex --force && mix local.rebar --force

RUN install -d /dashboard
