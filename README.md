
# nvoid
nvoid is a custom xbps-src repo which includes packages which can not be accepted into [void-packages](https://github.com/void-linux/void-packages/) or just experimental and WIP.

## supported architectures
all packages support `x86_64` (glibc), most of them support `x86_64-musl`. others has not tested yet.

## quick start

fetch void-packages tree first
```
git clone --depth 1 https://github.com/void-linux/void-packages
```
fetch nvoid as well
```
git clone --depth 1 https://github.com/not-void/nvoid
```
merge them
```
cp -r nvoid/srcpkgs/*  void-packages/srcpkgs
cat nvoid/custom-shlibs >> void-packages/etc/shlibs
```
install `xtools` and `base-devel`
```
xbps-install base-devel xtools
```
build `pkgname` and install it
```
cd void-packages
./xbps-src pkg <pkgname>
xi <pkgname>
```

