# Maintainer: nihilowy <nihilowy at gmail dot com>
# Maintainer: christianbundy <christianbundy@fraction.io>

pkgname=surfer
pkgver=1
pkgrel=1
pkgdesc="personal fork of nihilowy's basic webkit2gtk browser"
arch=('i686' 'x86_64')
url="https://github.com/christianbundy/surfer"
license=('GPL')
makedepends=('git')
depends=('webkit2gtk')

source=("git+https://github.com/christianbundy/surfer.git")

build() {
	cd "$pkgname"
	make
}

package() {
	cd "$pkgname"
	DESTDIR="${pkgdir}/opt/$pkgname" make install
}
md5sums=('SKIP')
