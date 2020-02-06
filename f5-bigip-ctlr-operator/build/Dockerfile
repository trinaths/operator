FROM quay.io/operator-framework/helm-operator:v0.12.0

### Required OpenShift Labels
LABEL name="F5 BIG-IP Controller Operator" \
      vendor="F5 Networks Inc" \
      version="v1.0.0" \
      release="1" \
      summary="This is an example of a wordpress helm operator." \
      description="This operator will deploy wordpress to the cluster."

# Required Licenses
COPY licenses /licenses

COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts/ ${HOME}/helm-charts/
