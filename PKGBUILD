# Maintainer: xantares <xantares09 at hotmail dot com>

pkgname=ttimg-utils
pkgver=1
pkgrel=2
pkgdesc="Tools to manipulate the ttsystem OS file of TomTom devices (mkttimage/ttimgextract)"
arch=('i686' 'x86_64')
url="https://github.com/Rupan/tomtom"
license=('GPL')
depends=('glibc')
makedepends=('gcc' 'make' 'git')
source=("git://github.com/Rupan/tomtom")
md5sums=('SKIP')

build() {
  cd "$srcdir/tomtom"
  ./build.sh
}

package() {
  cd "$srcdir/tomtom"
  install -d "$pkgdir"/usr/bin
  install -m 755 mkttimage ttimgextract "$pkgdir"/usr/bin
}
