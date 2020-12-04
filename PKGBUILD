# Maintainer: Twingate <v.hrytsiienko@gmail.com>

pkgname=twingate-bin

pkgver=0.46.0
_pkgver=_gOnZV

pkgrel=1
pkgdesc="Twingate Linux Client Twingate Linux Client"
arch=('x86_64')
depends=('dbus' 'libnl' 'networkmanager' 'python' 'libcurl-gnutls')
provides=("twingate")
conflicts=("twingate")
url='https://twingate.com/'
source=("https://packages.twingate.com/apt/files/ver$_pkgver/twingate-amd64.deb")
sha256sums=('6610c81c491f107cecc2444956f78a15147c6abbd547452023b7735e785f5417')

package() {
  bsdtar -xv -C "${pkgdir}" -f "${srcdir}/data.tar.gz"
  rm -rf ${pkgdir}/run
}
