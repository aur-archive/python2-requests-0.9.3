pkgname=python2-requests-0.9.3
pkgver=0.9.3
pkgrel=2
pkgdesc="Python HTTP for Humans."
url="http://python-requests.org"
depends=('python2' )
makedepends=('python2-distribute' )
optdepends=('python2-certifi: SSL support')
license=('custom: ISC')
arch=('any')
source=("http://pypi.python.org/packages/source/r/requests/requests-$pkgver.tar.gz")
conflicts=('python2-requests' 'python2-requests-0.10.0')
provides=('python2-requests')
build() {
    cd $srcdir/requests-$pkgver
    python2 setup.py build
}

package() {
    cd $srcdir/requests-$pkgver
    python2 setup.py install --root="$pkgdir" --optimize=1
}

md5sums=('b13b6fbfa8fc3fc3c25bae300748053f')
