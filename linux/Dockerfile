FROM zoobab/openwrt-daily-trunk-ar71xx-toolchain

USER openwrt
WORKDIR /home/openwrt/openwrt
RUN make tools
RUN make -j`nproc` || make -j1 V=s
