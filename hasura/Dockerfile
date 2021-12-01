FROM hasura/graphql-engine:v2.0.4
RUN apt update
RUN apt install curl -y
RUN curl -L https://github.com/hasura/graphql-engine/raw/stable/cli/get.sh | bash
ADD ./hasura $HOME/bdjuno/hasura
RUN cd /bdjuno/hasura
RUN hasura metadata apply --endpoint http://localhost:8080

