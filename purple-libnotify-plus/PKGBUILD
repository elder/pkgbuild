# Maintainer:  Elder Marco <eldermarco at gmail dot com>

pkgname=purple-libnotify-plus
pkgver=1.99.2
pkgrel=1
pkgdesc="Provide libnotify interface to Pidgin and Finch"

license=('GPL3')
url="https://github.com/sardemff7/purple-libnotify-plus"
source=("https://github.com/downloads/sardemff7/$pkgname/$pkgname-$pkgver.tar.xz")

makedepends=('glib2' 'libnotify>=0.6.0' 'libpurple>=2.6.0' 'purple-events' 'perl-xml-parser' 'intltool>=0.35.0')
options=(!libtool)

depends=('glib2' 'libnotify>=0.6.0' 'libpurple>=2.6.0' 'purple-events')

arch=('i686' 'x86_64')
md5sums=('94fd193a269b6ba188d45121c128a6e1')

build () {
    cd "$srcdir/$pkgname-$pkgver"

    ./configure --prefix=/usr
    make
}

package () {
    cd "$srcdir/$pkgname-$pkgver"
    make DESTDIR="$pkgdir" install
}
# expandtab:tabstop=4:shiftwidth=4
