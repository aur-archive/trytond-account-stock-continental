# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-account-stock-continental
_pkgname=trytond_account_stock_continental
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The account_stock_continental module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-account>=3.4' 'trytond-account-product>=3.4' 'trytond-stock>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("d7ee8bc158c739158d13254922b3fb13")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}