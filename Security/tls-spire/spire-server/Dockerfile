FROM gcr.io/spiffe-io/spire-server:1.0.1

# Override spire configurations
COPY conf/spire-server.conf /opt/spire/conf/server/server.conf
COPY conf/ca.crt /opt/spire/conf/server/agent-cacert.pem

WORKDIR /opt/spire
