FROM registry.gitlab.com/distribworks/dkron-pro:4.0.0-beta5

# config
COPY dkron.yml /etc/dkron/dkron.yml

# policies
COPY default.json /opt/local/dkron/policies/default.json
COPY readonly.json /opt/local/dkron/policies/readonly.json
