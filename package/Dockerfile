FROM ghcr.io/oracle/oraclelinux:7-slim

RUN yum update -y

COPY bin/rancher-operator /usr/bin/
COPY LICENSE README.md.in THIRD_PARTY_LICENSES.txt SECURITY.md /licenses/

USER 1000
CMD ["rancher-operator"]
