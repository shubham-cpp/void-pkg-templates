# void-pkg-templates
Custom templates for several packages that could be installed using xbps-src

# Installation Process
```bash
# I would Highly recommend to install xtools
sudo xbps-install -S xtools
git clone git://github.com/void-linux/void-packages.git ~/void-packages
```

## Post Install
```bash
cd ~/void-packages
./xbps-src binary-bootstrap
```

# How To use these custom templates
```bash
git clone https://github.com/shubham-cpp/void-pkg-templates /tmp/void-templates
cp -r /tmp/void-templates/* --target-directory void-packages/srcpkgs
./xbps-src pkg <package_name>
sudo xi <package_name>
```

# Template Packages Description

- [xcolor](https://github.com/Soft/xcolor) : Simple X color picker written in rust
- [xplr](https://github.com/sayanarijit/xplr) : A hackable, minimal, fast TUI file explorer

# References
- https://github.com/void-linux/void-packages
- https://github.com/void-linux/void-packages/blob/master/Manual.md
- https://re00.home.blog/2019/06/15/create-new-xbps-src-package/
