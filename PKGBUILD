# Maintainer: Lost Souls Guild - Nemesis <lost.souls.nemesis@gmail.com>
pkgname=ajour-bin
pkgver=0.3.4
pkgrel=1
pkgdesc="Ajour is a World of Warcraft addon manager written in Rust with a strong focus on performance and simplicity"
arch=('x86_64')
url="https://www.getajour.com/"
license=('MIT')
depends=('fontconfig' 'openssl' 'libxcb' 'vulkan-tools' 'vulkan-icd-loader')
makedepends=('git')
optdepends=('vulkan-intel' 'nvidia-utils' 'vulkan-radeon')
backup=()
provides=('ajour')
conflicts=('ajour')
source=(
  "https://github.com/lostsoulsnemesis/ajour-bin/releases/download/${pkgver}/ajour"
  "https://github.com/lostsoulsnemesis/ajour-bin/releases/download/${pkgver}/LICENSE"
)
md5sums=('6869249cadd50e377c4c025abf597047' 'fef427a98704a99573848b4b163426e3')
install="ajour.install"
	 
package() {
  install -D -m755 "${srcdir}/ajour" "${pkgdir}/usr/bin/ajour"
  install -D -m644 "${srcdir}/LICENSE" "${pkgdir}/usr/share/licenses/ajour/LICENSE"
}
