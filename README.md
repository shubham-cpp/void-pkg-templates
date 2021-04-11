# void-pkg-templates
Custom templates for several packages that could be installed using xbps-src

# installation process
```bash
# I would Highly recommend to install xtools
 sudo xbps-install -S xtoos
 git clone git://github.com/void-linux/void-packages.git
 cd void-packages
 ./xbps-src binary-bootstrap
 echo XBPS_ALLOW_RESTRICTED=yes >> etc/conf
 git clone https://github.com/shubham-cpp/void-pkg-templates ~/Download/templates
 cp -r ~/Downloads/templates/* --target-directory void-packages/srcpkgs
 ./xbps-src pkg <package_name>
 sudo xi <package_name>
```

# Template Packages Description

1. [xcolor](https://github.com/Soft/xcolor) : Simple X color picker written in rust
2. [vpm](https://github.com/netzverweigerer/vpm) : An XBPS package management helper for VoidLinux. For some reason the default vpm package doesn't have bash completion, so added it
