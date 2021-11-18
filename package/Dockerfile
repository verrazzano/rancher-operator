# Copyright (C) 2021, Oracle and/or its affiliates.
# Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl.

FROM ghcr.io/oracle/oraclelinux:7-slim

RUN yum update -y && yum-config-manager --enable ol7_u8_security_validation && \
    yum update -y openssl-libs

COPY bin/rancher-operator /usr/bin/
COPY LICENSE README.md.in THIRD_PARTY_LICENSES.txt SECURITY.md /licenses/

USER 1000
CMD ["rancher-operator"]
