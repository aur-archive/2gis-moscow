pkgname=2gis-moscow
pkgver=27
pkgrel=1
pkgdesc="Map of Moscow for 2GIS, July 2013"
arch=('i686' 'x86_64')
url="http://msk.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Moscow-27.orig.zip")
md5sums=('6a538efe95470454059e357c0d3adc0c')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Moscow.dgdat" "${pkgdir}/opt/2gis/moscow.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Moscow.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/moscow.dglf" || return 1
}
