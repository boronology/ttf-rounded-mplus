# Maintainer : boronology
pkgname=ttf-rounded-mplus
pkgver=1.056.20130705
pkgrel=1
depends=('fontconfig' 'xorg-font-utils')
pkgdesc="Rounded style gothic fonts based on M+ FONTS"
arch=('any')
license=('custom')
url="https://sites.google.com/site/roundedmplus/"
source=(https://googledrive.com/host/0B5ofAkcx0d7udkRiMDJxbGFFZ0U
	https://googledrive.com/host/0B5ofAkcx0d7uT0E1d01NUzVqNk0
	https://googledrive.com/host/0B5ofAkcx0d7uWjRoQkdrVHNQaTQ
	)

install=$pkgname.install

package() {
	cd "$srcdir"
	for TTF in `ls | grep ttf`
	    do
	    install -Dm644 $TTF "$pkgdir/usr/share/fonts/TTF/$TTF"
	    done
	for LICENSE in `ls mplus-TESTFLIGHT-056 | grep LICENSE`
	    do
	    install -Dm 644 mplus-TESTFLIGHT-056/$LICENSE "$pkgdir/usr/share/licenses/$pkgname/$LICENSE"
	    done
}
	    
md5sums=('365f183cd2dee894e95fe85cafe56470'
         'bdf827295e3123175882c982874b3b0c'
         '395be604e98688bf2e40ded94122997d')

