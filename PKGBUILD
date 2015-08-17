# Maintainer: Ivan Pulido < ijpulidos at riseup.net >

pkgname=python-plotly
pkgver=1.4.14
pkgrel=2
pkgdesc='Python API for Plotly, a collaborative data analysis and graphing tool on the cloud.'
arch=('any')
url='https://plot.ly/'
license=('MIT')
depends=('python' 'python-requests' 'python-six' 'python-pytz')
source=("https://pypi.python.org/packages/source/p/plotly/plotly-${pkgver}.tar.gz")
md5sums=('123502aa9ed45409dab94178c2767e64')

build() {
  cd plotly-${pkgver}

  python setup.py build
}

package() {
  cd plotly-${pkgver}

  python setup.py install \
    --root ${pkgdir}
}
