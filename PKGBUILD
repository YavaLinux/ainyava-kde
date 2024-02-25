# Maintainer: Hamed Mahmoudkhani <ainyava@gmail.com>
pkgname=ainyava-kde-git
pkgver=1.0.0
pkgrel=1
epoch=
pkgdesc="Ainyava theme for KDE Plasma 5"
arch=('any')
url="https://github.com/yavalinux/ainyava-kde"
license=('GPL3')
groups=()
depends=()
makedepends=('git')
checkdepends=()
optdepends=(
	'konsole: for konsole theme'
	'kvantum: for kvantum theme (recommended)'
	'plasma-desktop: for plasma desktop theme'
)
provides=("$pkgname=$pkgver")
conflicts=("$pkgname")
replaces=()
backup=()
options=()
install=
changelog=
source=("$pkgname::git+$url.git")
noextract=()
sha256sums=('SKIP')
validpgpkeys=()

prepare() {
	cd "$pkgname"
}

package() {
	cd "$pkgname"
	make DESTDIR="$pkgdir/" install
}
