Step 1. Prerequisites

```bash
sudo apt-get install -y libgcrypt20 libglib2.0-0 libpixman-1-0 libsdl2-2.0-0 libslirp0
```

Step 2. Set-up qemu
```bash
./configure --target-list=riscv32-softmmu \
    --enable-gcrypt \
    --enable-slirp \
    --enable-debug --enable-sanitizers \
    --enable-sdl \
    --disable-strip --disable-user \
    --disable-capstone --disable-vnc \
    --disable-gtk
```

```bash
ninja -C build
```
