# Contributor: Xavion <Xavion (dot) 0 (at) Gmail (dot) com>
# Contributor: damir <damir@archlinux.org>

pkgname=zsync
pkgver=0.6.2
pkgrel=1
pkgdesc="A file transfer program that's able to connect to rsync servers"
arch=("i686" "x86_64")
url="http://zsync.moria.org.uk/"
depends=("glibc")
license=("artistic")
#source=(http://belnet.dl.sourceforge.net/sourceforge/${pkgname}/${pkgname}-${pkgver}.tar.gz)
source=(http://${pkgname}.moria.org.uk/download/${pkgname}-${pkgver}.tar.bz2)

build() {
	cd "${srcdir}"/${pkgname}-${pkgver}

	./configure --prefix=/usr
	make
}

package() {
	cd "${srcdir}"/${pkgname}-${pkgver}

	make prefix="${pkgdir}"/usr install
}

sha1sums=('5e69f084c8adaad6a677b68f7388ae0f9507617a')
