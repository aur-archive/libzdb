pkgname=libzdb
pkgver=2.9
pkgrel=1
pkgdesc="Zild Database Library"
arch=(i686 x86_64)
url="http://www.tildeslash.com/libzdb/"
license=('GPL')
depends=('postgresql-libs' 'sqlite3' 'libmysqlclient')
source=(http://www.tildeslash.com/libzdb/dist/libzdb-$pkgver.tar.gz)
md5sums=('8478e36a0f74dd93b810f12baa81afe0')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  ./configure --prefix=/usr
  make
  make DESTDIR="$pkgdir/" install
}
