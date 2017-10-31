FROM gcscaglia/docker-svnserve

# Install crystal for building our hooks application
RUN echo "http://public.portalier.com/alpine/testing" >> /etc/apk/repositories \
  && wget "http://public.portalier.com/alpine/julien%40portalier.com-56dab02e.rsa.pub" \
  -O /etc/apk/keys/julien@portalier.com-56dab02e.rsa.pub

RUN apk update && apk add openssl gcc libc-dev libevent-dev pcre-dev crystal shards

ADD svnserve.conf /
ADD passwd /

CMD ["/usr/bin/svnserve", "--daemon", "--foreground", "--root", "/var/opt/svn", "--config-file", "/svnserve.conf", "--log-file", "/var/opt/svn/log"]
