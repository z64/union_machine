FROM base/archlinux

RUN pacman -Syu --noconfirm && \
    pacman -S --noconfirm \
           base-devel \
           crystal \
           shards \
           vim

VOLUME ["/data", "/union"]

ENTRYPOINT "/bin/bash"
