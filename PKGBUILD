# Maintainer: Ferrum-Language <noreply@ferrum-lang.org>
pkgname=ferrumc
pkgver=0.3.0
pkgrel=1
pkgdesc="Ferrum-language compiler — systems programming with compile-time memory safety"
arch=('x86_64' 'aarch64')
url="https://ferrum-language.github.io/Ferrum/"
license=('MIT')
depends=('llvm18-libs')
makedepends=()
provides=('ferrumc')
conflicts=()
source_x86_64=("${pkgname}-${pkgver}-linux-x86_64.tar.gz::https://github.com/Ferrum-Language/Ferrum/releases/download/v${pkgver}/ferrumc-v${pkgver}-linux-x86_64.tar.gz")
source_aarch64=("${pkgname}-${pkgver}-linux-aarch64.tar.gz::https://github.com/Ferrum-Language/Ferrum/releases/download/v${pkgver}/ferrumc-v${pkgver}-linux-aarch64.tar.gz")
sha256sums_x86_64=('1cea7ef7eb58426fe8ec5942d16bee985e218a5997028fc05f137a0c31dd405b')
sha256sums_aarch64=('9284560230b179cfa7d78dea6af1d1d3abd5379279e7aa8ecb2be8262e236fca')

package() {
    install -Dm755 ferrumc "${pkgdir}/usr/bin/ferrumc"
    install -Dm644 /dev/stdin "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE" <<'EOF'
MIT License — see https://github.com/Ferrum-Language/Ferrum/blob/main/LICENSE
EOF
}
