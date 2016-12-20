# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Salty Blu <s.blu24@gmail.com>
pkgname=mario
pkgver=1.0
pkgrel=1
epoch=0
pkgdesc=""
arch=(x86_64)
url=""
license=('MirOS Licence')
groups=()
depends=(pkgfile yaourt)
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(https://github.com/sblu/mario/archive/1.0.zip)
noextract=()
md5sums=(3a9f009f916f435af1742d1bc01a2ada)

prepare() {
    echo "Preparing..."
}

build() {
    echo "Building..."
}

check() {
    echo "Checking..."
}

package() {

    mkdir -p $pkgdir/usr/bin/
    mkdir -p $pkgdir/var/lib/mario/bin
    mkdir -p $pkgdir/var/lib/mario/completions
    mkdir -p $pkgdir/var/lib/mario/libexec
    mkdir -p $pkgdir/var/lib/mario/share

    cd "$pkgname-$pkgver"

    cp bin/mario $pkgdir/var/lib/mario/bin/mario
    cp -r completions/* $pkgdir/var/lib/mario/completions
    cp -r libexec/* $pkgdir/var/lib/mario/libexec
    cp -r share/* $pkgdir/var/lib/mario/share
    cp -r LICENSE $pkgdir/var/lib/mario
    ln -sf /var/lib/mario/bin/mario $pkgdir/usr/bin/mario
}
