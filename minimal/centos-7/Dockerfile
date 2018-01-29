FROM centos:7
MAINTAINER SaltStack, Inc.

# Install EPEL
RUN yum -y install epel-release

# Update Current Image
RUN yum install -y libcom_err && yum update -y

# Install Salt Dependencies
RUN yum -y install --enablerepo=epel \
  python \
  PyYAML \
  m2crypto \
  python-crypto \
  python-msgpack \
  python-zmq \
  python-setuptools

RUN easy_install \
  jinja2 \
  requests
