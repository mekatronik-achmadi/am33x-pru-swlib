pkgname=am33x-pru-swlib
pkgver=2.0.1.1
pkgrel=1
pkgdesc="PRU C library from StarterWare"
arch=('any')
url="https://github.com/BeaglePilot/PRUSS-C"
license=('GPL')
depends=('am33x-pru-cc')
makedepends=()
options=('!makeflags' '!strip' 'staticlibs' 'libtool')
source=("$pkgname::git+https://github.com/mekatronik-achmadi/am33x-pru-swlib")
sha256sums=('SKIP')

package() {
	cd "$srcdir/$pkgname"

	install -d $pkgdir/opt/pru-cc/
	mv -vf am335x_starterware $pkgdir/opt/pru-cc/
}
