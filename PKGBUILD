# Maintainer: Walter Broemeling <wallebroem at gmail dot com>

pkgname=w-help-git
_name=w-help
pkgver=r2.9275fc8
pkgrel=1
pkgdesc="Walter\'s help script, for noobs."
arch=("any")
url="https://github.com/WTechNinja/w-help"
license=('Unlicense')
depends=('bash')
makedepends=('git' 'gzip')
provides=('w-help')
conflicts=('w-help')
source=("git+$url.git")
noextract=()
md5sums=('SKIP')

pkgver() {
        cd "$_name"
        printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
        # Script
        cd "$_name"
        install -Dm755 help "$pkgdir/usr/bin/help"
}
