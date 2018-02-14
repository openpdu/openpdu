# Contributor: Paolo Asperti <paolo@asperti.com>
# Maintainer: Paolo Asperti <paolo@asperti.com>
pkgname=openpdu
pkgver=0.1
pkgrel=1
pkgdesc="OpenPDU project - main binary"
url="https://github.com/paspo/installinux"
arch="noarch"
license="GPL2"
depends="python, py-argh, apk-cron"
makedepends=""
install="openpdu.post-install"
subpackages=""
source=""

build() {
	:
}

package() {
	mkdir -p "$pkgdir"
	install -Dm644 etc/openpdu/openpdu.conf "$pkgdir"/etc/openpdu/openpdu.conf
	install -Dm755 etc/local.d/openpdu.start "$pkgdir"/etc/local.d/openpdu.start

	install -Dm755 openpdu "$pkgdir"/usr/sbin/openpdu
}
