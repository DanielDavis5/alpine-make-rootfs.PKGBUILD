# Maintainer: Daniel Maurice Davis <daniel.maurice.davis@gmail.com>
_program=alpine-make-rootfs
_coder=DanielDavis5

pkgname="$_program-$_coder"
pkgver=0.5.1
pkgrel=1
pkgdesc="Builds customized Alpine Linux rootfs for containers."
arch=('any')
source=("$_program-$pkgver.tar.gz::https://github.com/$_coder/$_program/archive/v$pkgver.tar.gz")
license=('MIT')
md5sums=('7038273c5fff0cef2dda334a72141dde')
provides=("$_program")

package() {
	cd "$_program-$pkgver"
	make DESTDIR="$pkgdir/" install
}
