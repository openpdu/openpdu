# Contributor: Paolo Asperti <paolo@asperti.com>
# Maintainer: Paolo Asperti <paolo@asperti.com>
pkgname=openpdu
pkgver=0.2.0
pkgrel=1
pkgdesc="OpenPDU project - main binary"
url="https://github.com/openpdu/openpdu"
arch="noarch"
license="GPL2"
depends="python py-argh apk-cron py-bottle i2c-tools"
makedepends=""
install="openpdu.post-install"
subpackages=""
source=""
options="!check"

build() {
	:
}

package() {
	mkdir -p "$pkgdir"
	install -Dm644 etc/openpdu/boards.conf "$pkgdir"/etc/openpdu/boards.conf
	install -Dm644 etc/openpdu/outlets.conf "$pkgdir"/etc/openpdu/outlets.conf
	install -Dm755 etc/local.d/openpdu.start "$pkgdir"/etc/local.d/openpdu.start

	install -Dm755 openpdu "$pkgdir"/usr/bin/openpdu
	install -Dm755 openpdud "$pkgdir"/usr/bin/openpdud
}
