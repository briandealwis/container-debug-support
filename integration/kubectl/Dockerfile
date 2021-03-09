ARG GOVERSION
FROM --platform=$BUILDPLATFORM curlimages/curl
ARG BUILDPLATFORM
ARG TARGETOS
ARG TARGETARCH
USER root
ADD https://dl.k8s.io/release/v1.20.0/bin/$TARGETOS/$TARGETARCH/kubectl /usr/bin
RUN chmod a+x /usr/bin/kubectl
ENTRYPOINT ["/usr/bin/kubectl"]
