# Maintainer: 0xMRTT < 0xMRTT at proton dot me >

pkgname="atrophaneura-wallpapers"
pkgver=0.1.0
pkgrel=2
pkgdesc='Atrophaneura project's Wallpapers'
arch=('any')
url="https://github.com/atrophaneura/Wallpapers"
license=('GPL')
source=("git+$url")
makedepends=('git')
sha256sums=('SKIP')

package() {
    cd "$srcdir/Wallpapers"

    find . \
        -type f \
     \( -name "*.png" -o -name "*.svg" \) \
        -exec install -Dm 0755 -t "$pkgdir/usr/share/backgrounds/atrophaneura/." {} +
}
