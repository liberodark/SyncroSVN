# Maintainer: liberodark

pkgname=syncrosvn
pkgver=10.1
pkgrel=1
pkgdesc="Syncro SVN Client has been designed to offer powerful actions while keeping the interface as clean and simple as possible."
arch=('x86_64')
url="http://www.syncrosvnclient.com/"
license=('custom')
depends=('xdg-utils' 'jre8-openjdk')
source_x86_64=("http://www.syncrosvnclient.com/InstData/All/syncroSVNClient.tar.gz")
source=($pkgname.desktop
        $pkgname.png)
sha512sums=('f7a28907a9d6e08edac19adbd7016f2d6f31fe2944a4fc073aff1662e11c98eb1f386acffee75ba56b5324fb8a0ac6de089458b6cbc0000b07bfe19167e225d9'
         'd063dd4f8d620c759ff15637bd1d5f23ce7c11b85a45b55ecd1d62fbde390cdf360110dbf7ff1d7776484ea1f485f4bbf2915cf1212ceec9ac323a2ef2e71aef')
sha512sums_x86_64=('169f98334005b3876ad7db70ae7c446c17ef9f508f75602c75243a2f59776479c4d184707f101861db53660e8bd7bafb17ebcac9986c911b73d900f580909916')
        
package() {
  cd $srcdir
  tar xvf syncroSVNClient.tar.gz
  mkdir -p "$pkgdir/usr/bin/syncrosvn/"
  cp -r "syncroSVNClient/." "$pkgdir/usr/bin/syncrosvn/"
  install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}
