# Data Volume Container for Magento and MySQL
FROM scratch
MAINTAINER Abdullah <abdullah.rayeen@gmail.com>
COPY . /
# Hack for https://github.com/docker/fig/pull/517
COPY true-asm /bin/echo
VOLUME ["/srv/magento", "/var/lib/mysql"]
# Executables this small
# Thanks to tianon
# Haiku by way of credit
# https://github.com/tianon/dockerfiles
ENTRYPOINT ["/sleeping-beauty"]
