# DOCKER-VERSION 1.0.0
#
# Ceph All In One
#
# VERSION 0.0.1

FROM ceph/base
MAINTAINER Sébastien Han "seb@redhat.com"

# Add bootstrap script
ADD entrypoint.sh /entrypoint.sh

# Add volumes for Ceph config and data
VOLUME ["/etc/ceph","/var/lib/ceph"]

# Expose the Ceph ports
EXPOSE 6789
EXPOSE 6800
EXPOSE 6801
EXPOSE 6802
EXPOSE 6803
EXPOSE 6804
EXPOSE 6805
EXPOSE 80

# Execute monitor as the entrypoint
ENTRYPOINT ["/entrypoint.sh"]
