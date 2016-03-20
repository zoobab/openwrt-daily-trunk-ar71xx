FROM zoobab/openwrt-daily-trunk-ar71xx-tools

RUN make -j`nproc` toolchain/install || make -j1 V=s
