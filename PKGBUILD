# Maintainer: NicoHood <archlinux {cat} nicohood {dog} de>
# PGP ID: 97312D5EB9D7AE7D0BD4307351DAE9B7C1AE9161

pkgname=nicohood
_pkgname=archlinux
pkgver=0.0.9
pkgrel=1
pkgdesc="A collection of personal Arch Linux tools."
arch=('any')
url="https://github.com/NicoHood"
license=('GPL3')
depends=('bash' 'arch-install-scripts' 'btrfs-progs' 'dosfstools' 'cryptsetup')
source=("${pkgname}-${pkgver}.tar.xz::https://github.com/NicoHood/${_pkgname}/releases/download/${pkgver}/${_pkgname}-${pkgver}.tar.xz"
        "${pkgname}-${pkgver}.tar.xz.asc::https://github.com/NicoHood/${_pkgname}/releases/download/${pkgver}/${_pkgname}-${pkgver}.tar.xz.asc")
sha512sums=('79a49ff6c283b5efbe854bec3937d1220f94fbe83d27de4025cea732619522312aed411c0731861ba357ee37f53a17eebfdb11c6cba622fcbe8811dcbfbe5950'
            'SKIP')
# NicoHood <archlinux {cat} nicohood {dog} de>
validpgpkeys=('97312D5EB9D7AE7D0BD4307351DAE9B7C1AE9161')

package() {
    make -C "${_pkgname}-${pkgver}" DESTDIR="${pkgdir}" install
}
