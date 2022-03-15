# Maintainer: Hoàng Văn Khải <hvksmr1996@gmail.com>

pkgname='dprint-bin'
pkgver='0.23.1'
pkgrel='1'
pkgdesc='Pluggable and configurable code formatting platform written in Rust.'
arch=('x86_64')
url='https://dprint.dev/'
license=('MIT')
_repo='https://github.com/dprint/dprint'
source=(
  "$pkgver.zip::$_repo/releases/download/$pkgver/dprint-x86_64-unknown-linux-gnu.zip"
  "$pkgver.LICENSE::$_repo/raw/$pkgver/LICENSE"
)
sha256sums=(
  'c57923a76ce8b5b134371f337db437a59b4ea5a86875c55339d366ad409bfd2a'
  'SKIP'
)

package() {
  install -Dm755 dprint "$pkgdir/usr/bin/dprint"
  install -Dm644 "$pkgver.LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
