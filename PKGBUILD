pkgname=xerox-docucentre-util
pkgver=1.0.0
_pkgver=1.1.1-1
pkgrel=1
pkgdesc="Utility for the Fuji-Xerox DocuCentre series. Also supports ApeosPort and DocuPrint series."
url="https://www.fujixerox.co.jp/download/docuprint/download/p450d/linux_utility64"
license=('custom')
arch=('x86_64')
depends=('cups' 'tcl' 'tk')
source=(http://download.fujixerox.co.jp/pub/exe/docuprint/p450d/fxlinuxprintutil-${_pkgver}.x86_64.rpm)
md5sums=('84edca7b7d3cf0fba26a10b2098d285c')

package() {
	cd "${srcdir}"

	rm -rf "${srcdir}"/usr/lib64
	cp -R "${srcdir}"/usr "${pkgdir}"
}
