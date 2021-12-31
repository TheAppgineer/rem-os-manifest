# rem-os-manifest
```shell
curl https://storage.googleapis.com/git-repo-downloads/repo > repo
chmod +x repo
sudo mv repo /usr/local/bin/

mkdir rem-os
cd rem-os
repo init -u https://github.com/TheAppgineer/rem-os-manifest.git -b honister
repo sync

TEMPLATECONF=meta-rem-os/conf/samples/ source oe-init-build-env
bitbake rem-os-image-develop
```
