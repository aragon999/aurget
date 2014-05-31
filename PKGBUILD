# Author: Patrick Brisbin <pbrisbin@gmail.com>
pkgname=aurget
pkgver=4.2.0
pkgrel=1
pkgdesc="A simple Pacman-like interface to the AUR"
arch=('any')
url="https://github.com/pbrisbin/$pkgname"
license=('GPL')
install=$pkgname.install
source=(
  $pkgname
  ${pkgname}.1
  ${pkgname}rc.5
  ${pkgname}rc
  bash_completion
  zsh_completion
)
optdepends=('customizepkg: for auto-customizing packages')

package() {
  install -Dm755 $pkgname        "$pkgdir/usr/bin/$pkgname"
  install -Dm644 ${pkgname}.1    "$pkgdir/usr/share/man/man1/${pkgname}.1"
  install -Dm644 ${pkgname}rc.5  "$pkgdir/usr/share/man/man5/${pkgname}rc.5"
  install -Dm644 ${pkgname}rc    "$pkgdir/usr/share/doc/aurget/samples/${pkgname}rc"
  install -Dm644 bash_completion "$pkgdir/etc/bash_completion.d/aurget"
  install -Dm644 zsh_completion  "$pkgdir/usr/share/zsh/site-functions/_aurget"
}
md5sums=('b6e9704c9874d8a5abba3eccfa9ea240'
         'd41d8cd98f00b204e9800998ecf8427e'
         '3726da3816919d2c309668246e9d9c02'
         '976b2de0e15fd87316d16543be53b208'
         '2d33fc9c6d8b8c9219c7a91c90f328bc'
         'e8df58f145a7d487cccb0e7f6b1ec8aa')
