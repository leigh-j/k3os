### BASE ###
FROM alpine:3.11 as base
ARG ARCH
RUN apk --no-cache add \
    $([ "$ARCH" == "amd64" ] && echo "open-vm-tools grub-bios") \
    bash \
    bash-completion \
    blkid \
    busybox-initscripts \
    ca-certificates \
    connman \
    conntrack-tools \
    coreutils \
    curl \
    dbus \
    dosfstools \
    e2fsprogs \
    e2fsprogs-extra \
    efibootmgr \
    eudev \
    findutils \
    grub-efi \
    haveged \
    htop \
    hvtools \
    iproute2 \
    iptables \
    iscsi-scst \
    jq \
    kbd-bkeymaps \
    logrotate \
    lsscsi \
    lvm2 \
    lvm2-extra \
    mdadm \
    mdadm-misc \
    mdadm-udev \
    multipath-tools \
    ncurses \
    nfs-utils \
    open-iscsi \
    openrc \
    openssh-client \
    openssh-server \
    parted \
    procps \
    qemu-guest-agent \
    rng-tools \
    rsync \
    strace \
    sudo \
    tar \
    util-linux \
    vim \
    xz \
 && mv -vf /etc/conf.d/qemu-guest-agent /etc/conf.d/qemu-guest-agent.orig \
 && mv -vf /etc/conf.d/rngd             /etc/conf.d/rngd.orig \
 && mv -vf /etc/conf.d/udev-settle      /etc/conf.d/udev-settle.orig \
 && true
