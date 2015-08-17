# Maintainer: Andy Weidenbaum <archbaum@gmail.com>

pkgname=nodejs-bitcoin
_npmname=bitcoin
pkgver=2.2.0
pkgrel=1
pkgdesc="Communicate with bitcoind via JSON-RPC"
arch=('any')
depends=('nodejs')
makedepends=('npm')
url="https://github.com/freewil/node-bitcoin"
license=('MIT')
provides=('nodejs-bitcoin')

package() {
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p "$_npmdir"
  cd "$_npmdir"
  npm install --user root -g --prefix "$pkgdir/usr" $_npmname@$pkgver
}
