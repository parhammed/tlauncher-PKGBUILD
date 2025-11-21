# Maintainer: Parham Taki <parhammed@gmail.com>

pkgname=tlauncher
pkgver=16
pkgrel=1
pkgdesc="TLAUNCHER – THE BEST MINECRAFT LAUNCHE"
arch=('any')
conflicts=(tlauncher)
depends=(
	'jdk8-openjdk'
	'jre8-openjdk' 
	'jre8-openjdk-headless'
)
url="https://tlauncher.org/"
license=('none') # I have no idea if it has a license or no (probably not)
options=(!debug)
source=(
	"tlauncher.zip::https://dl1.tlauncher.org/f.php?f=files%2FTLauncher.v${pkgver}.zip"
	"tlauncher.desktop"
	"tlauncher.png"
)
sha512sums=(
	'7151fb3739d394775b4c3400524af9442a09b25fbc59778b9dfcc23d976fd5f463eca7e05a2dcd3d8b7a769bee55b28e216769e604dd243629f9b3b519d32cb6'
	'2a363f472e74394a4deabaf1df06d6915ae9bcfb39a15c88bbd3eb07092524571f105440965b0f639714e8e76fe11251b36436aefe2a2cb5f170a7df6098e84b'
	'663874b9a5fa10ceb794b30e66f7ab87820b80cfe136b967b492074e7dbce4173860e344c46cb25d2b8a52ea8a8ff2abfafaad9276462dcd4dd1b3e55819d9ac'
)

package() {
	install -Dm755 TLauncher.jar "$pkgdir/opt/tlauncher/TLauncher.jar"
	
	install -Dm755 tlauncher.desktop "$pkgdir/usr/share/applications/tlauncher.desktop"
   	install -Dm644 tlauncher.png "$pkgdir/usr/share/icons/tlauncher.png"	
}
