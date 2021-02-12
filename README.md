
# nvoid
nvoid is a custom xbps-src repo that includes packages which can not be accepted into [void-packages](https://github.com/void-linux/void-packages/). 

## supported architectures
all packages **must** support `x86_64-glibc` (with exception of *-bin)
- [X] x86_64-glibc
- [ ] x86-64-musl
- [ ] i686-glibc
- [ ] aarch64-glibc
- [ ] aarch64-musl

## quick start
`xtools` and `base-devel` are required for building and installing packages
```
xbps-install base-devel xtools
```
clone repo and bootstrap
```
git clone --depth 1 https://github.com/not-void/void-packages
cd nvoid
./xbps-src binary-bootstrap
```
build `pkgname` and install it
```
./xbps-src pkg <pkgname>
xi <pkgname>
````
