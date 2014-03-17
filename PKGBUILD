# Maintainer : boronology <boronology at gmail dot com>
pkgname=ttf-rounded-mplus
pkgver=1.058.20140226
pkgrel=1
depends=('fontconfig' 'xorg-font-utils')
pkgdesc="Japanese rounded gothic fonts based on M+ FONTS"
arch=('any')
license=('custom')
url="https://sites.google.com/site/roundedmplus/"
source=(https://googledrive.com/host/0B5ofAkcx0d7uWG0wVENtZjdmQ3M
	https://googledrive.com/host/0B5ofAkcx0d7uZzJIUUhhd1RUa2M
	https://googledrive.com/host/0B5ofAkcx0d7uWFlzcE94SnJveXc
	)

install=$pkgname.install

package() {
	cd "$srcdir"

	# install fonts
	for TTF in `ls | grep ttf`
	    do
	    install -Dm644 $TTF "$pkgdir/usr/share/fonts/TTF/$TTF"
	    done

	# install License
	for LICENSE in `ls mplus-TESTFLIGHT-058 | grep LICENSE`
	    do
	    install -Dm644 mplus-TESTFLIGHT-058/$LICENSE \
	    	    "$pkgdir/usr/share/licenses/$pkgname/$LICENSE"
	    done
}
	    
md5sums=('SKIP'
	'SKIP'
	'SKIP')

