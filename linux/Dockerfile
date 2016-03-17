FROM zoobab/openwrt-daily-trunk-ar71xx-toolchain

USER openwrt
WORKDIR /home/openwrt/openwrt
RUN make target/compile
RUN make package/compile
RUN make -j`nproc` || make -j1 V=s
