FROM quay.io/openshift/origin-must-gather:4.3.0 as builder

FROM centos:7

COPY --from=builder /usr/bin/oc /usr/bin/oc

COPY collection-scripts/* /usr/bin/

ENTRYPOINT /usr/bin/gather