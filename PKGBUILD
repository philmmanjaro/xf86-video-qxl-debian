pkgname=xf86-video-qxl-debian
# https://gitlab.freedesktop.org/xorg/driver/xf86-video-qxl/-/commits/master
_commit=52c421c650f8813665b31890df691b31fabc366a # master 2020-02-05
pkgver=0.1.5+git20200331
pkgrel=1
pkgdesc='Xorg X11 qxl video driver (Debian binary)'
arch=('x86_64')
url='https://www.x.org'
license=('MIT')
groups=('xorg-drivers')
depends=('spice')
optdepends=('python: for Xspice')
makedepends=('xorg-server-devel' 'X-ABI-VIDEODRV_VERSION=24.0' 'spice-protocol'
	'xorgproto' 'git' 'libcacard')
provides=(xf86-video-qxl)
conflicts=('xf86-video-qxl' 'xf86-video-qxl-git' 'X-ABI-VIDEODRV_VERSION<24' 'X-ABI-VIDEODRV_VERSION>=25')
source=("${pkgname}-${pkgver}-${pkgrel}.tar.gz")
sha256sums=('cfde73aa9f0544e65eab675878f671300bdaac25cced0a290c79486dec6a7e90')

package() {
	cd "${srcdir}/${pkgname}-${pkgver}-${pkgrel}"

	cp -av * "${pkgdir}"
}
