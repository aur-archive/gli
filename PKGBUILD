# Maintainer: Pablo Lluch <pablo.lluch@gmail.com>

pkgname=gli
pkgver=0.5.1.0
pkgrel=1
pkgdesc="C++ image library for 3D software based on OpenGL and GLSL conventions and used to load and store OpenGL textures."
arch=('any')
license=('MIT')
url="http://gli.g-truc.net"
depends=('glm')
source=("http://sourceforge.net/projects/ogl-image/files/gli-$pkgver/gli-$pkgver.zip")
md5sums=('79792e3afa93c7390d69cd21e4edd952')

package() {
    cd $pkgname-$pkgver
    mkdir -p $pkgdir/usr/include/gli
    cp -r gli $pkgdir/usr/include
    rm -f $pkgdir/usr/include/gli/CMakeLists.txt
    find $pkgdir -type f -exec chmod 644 {} \;
    find $pkgdir -type d -exec chmod 755 {} \;
}
