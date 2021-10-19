# Copyright (C) 2021, Oracle and/or its affiliates.
# Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl.

FROM ghcr.io/oracle/oraclelinux:7-slim

COPY bin/rancher-operator /usr/bin/
COPY LICENSE README.md.in THIRD_PARTY_LICENSES.txt SECURITY.md /license/

USER 1000
CMD ["rancher-operator"]
