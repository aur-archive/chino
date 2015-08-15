# Maintainer: David Adler <david dot jo dot adler at gmail dot com>
pkgname=chino
pkgver=0.20
pkgrel=1
pkgdesc="scripted session management for Linux audio"
arch=('any')
url="http://chino.tuxfamily.org/"
license=('GPL')
depends=('bc' 'graphviz' 'a2jmidid')
source=(http://download.tuxfamily.org/$pkgname/$pkgname-$pkgver.tar.bz2)
md5sums=('73899233bd02acd3ce93e4a333ded0ba')

build() {
	cd "$srcdir/$pkgname-$pkgver"
	./configure --prefix=/usr --sysconfdir=/etc 
}

package() {
	cd "$srcdir/$pkgname-$pkgver"
	make DESTDIR=$pkgdir install
}

# vim:set ts=2 sw=2 et:
