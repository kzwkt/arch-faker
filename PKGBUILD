# https://gitlab.archlinux.org/archlinux/packaging/packages/pkgname/-/blob/main/PKGBUILD?ref_type=heads

pkgname=base-busybox
pkgver=99
pkgrel=1
arch=('any')
depends=(
  'filesystem' 'gcc-libs' 'glibc' 
  'busybox'
  'shadow'
  'licenses' 'pacman' 'archlinux-keyring' 'systemd' 'systemd-sysvcompat'
)
provides=(base)


post_install() {
  # Install symlinks using busybox
  /usr/bin/busybox --install -s /usr/bin
  /usr/bin/busybox --install -s /usr/sbin
}
