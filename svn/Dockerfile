FROM gcscaglia/docker-svnserve

ADD svnserve.conf /
ADD passwd /

CMD ["/usr/bin/svnserve", "--daemon", "--foreground", "--root", "/var/opt/svn", "--config-file", "/svnserve.conf"]
