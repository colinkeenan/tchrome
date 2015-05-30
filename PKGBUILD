# Maintainer: Colin Keenan <colinnkeenan at gmail dot com>

pkgname=tchrome
pkgver=1.0
pkgrel=1
pkgdesc="Close Chrome browser including background, or launch a version of Google Chrome/Chromium"
arch=('any')
url="https://github.com/colinkeenan/tchrome"
license=('GPL')
install=${pkgname}.install

source=(https://raw.githubusercontent.com/colinkeenan/${pkgname}/v${pkgver}/${pkgname} 
        https://raw.githubusercontent.com/colinkeenan/${pkgname}/v${pkgver}/${pkgname}.conf 
	https://raw.githubusercontent.com/colinkeenan/${pkgname}/v${pkgver}/${pkgname}.desktop)
md5sums=('b37b1c2faa637744af0257f3f8546587'
         '3bab05dbc5357bbe934942503a79c6a3'
         'bbb853e12a46d832143a464377bc966d')

package() {
  install -D -m644 ${pkgname}.conf "$pkgdir/etc/${pkgname}.conf"
  install -D -m644 ${pkgname}.desktop "$pkgdir/usr/share/applications/${pkgname}.desktop"
  install -D -m755 ${pkgname} "$pkgdir/usr/bin/${pkgname}"
}
