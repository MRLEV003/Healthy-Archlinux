pkgname=healthy-archlinux-rust
pkgver=1.0.0
pkgrel=1
pkgdesc='Read-only system diagnostics for Arch Linux and Arch-based distributions (Rust edition)'
arch=('x86_64')
url='https://example.invalid/healthy-archlinux-rust'
license=('MIT')
depends=('glibc')
makedepends=('cargo')
source=()
sha256sums=()

build() {
  cd "$startdir"
  cargo build --release --locked
}

check() {
  cd "$startdir"
  cargo test --locked
}

package() {
  cd "$startdir"
  install -Dm755 target/release/hc-rs "$pkgdir/usr/bin/hc-rs"
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
