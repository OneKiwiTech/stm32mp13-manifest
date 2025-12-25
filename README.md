# stm32mp13-manifest

- `mkdir yocto-stm32mp13`
- `cd yocto-stm32mp13`
- `repo init -u https://github.com/OneKiwiTech/stm32mp13-manifest -b mickledore -m mp13-mickledore-mp1.xml`
- `repo sync -j8`
- `DISTRO=openstlinux-weston MACHINE=onekiwi source layers/meta-st/scripts/envsetup.sh build`
- `bitbake st-image-weston`