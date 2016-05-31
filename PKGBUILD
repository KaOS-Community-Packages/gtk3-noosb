pkgname=gtk3-noosb
pkgver=1.0
pkgrel=1
pkgdesc="Globally disable the GTK+3 overlay scrollbars"
arch=('x86_64')
url='https://blogs.igalia.com/carlosgc/category/free-software/gnome/'
license=('CC0')
depends=('gtk3')
makedepends=('coreutils')

package() {
	install -d "$pkgdir"/etc/profile.d
	cat <<\EOF >"$pkgdir"/etc/profile.d/gtk3-noosb.sh
export GTK_OVERLAY_SCROLLING=0
EOF
	chmod +x "$pkgdir"/etc/profile.d/gtk3-noosb.sh
}
