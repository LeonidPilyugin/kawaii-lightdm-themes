# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-lightdm-themes
pkgver=1.0
pkgrel=1
pkgdesc='Kawaii lightdm themes.'
depends=(lightdm lightdm-webkit2-greeter)
arch=('x86_64')
license=('GPL3')
groups=('kawaii')
source=("$pkgname-$pkgver.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('d32d066b9ebc9a3a9c77abd085a4f305194d0abf168b2b83a57fd82bb642314e')

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/usr/share/lightdm-webkit/themes/
    install -dm755 $dir
    cp -r $srcdir/* $dir
}

