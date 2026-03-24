# Maintainer: Ferrum-Language <noreply@ferrum-lang.org>
pkgname=ferrumc
pkgver=0.3.0
pkgrel=1
pkgdesc="Ferrum-language compiler — systems programming with compile-time memory safety"
arch=('x86_64' 'aarch64')
url="https://ferrum-language.github.io/Ferrum/"
license=('MIT')
provides=('ferrumc')
conflicts=()
source_x86_64=("${pkgname}-${pkgver}-linux-x86_64.tar.gz::https://github.com/Ferrum-Language/Ferrum/releases/download/v${pkgver}/ferrumc-v${pkgver}-linux-x86_64.tar.gz")
source_aarch64=("${pkgname}-${pkgver}-linux-aarch64.tar.gz::https://github.com/Ferrum-Language/Ferrum/releases/download/v${pkgver}/ferrumc-v${pkgver}-linux-aarch64.tar.gz")
sha256sums_x86_64=('2735cf702ff9c3f3bf9ad95140bde211f3e642590e9222800f81969727ea6029')
sha256sums_aarch64=('4324815376c13b8038705864805c4d5b0e44910b6cc52c3111ec311afcc4cf9c')

package() {
    install -Dm755 ferrumc "${pkgdir}/usr/bin/ferrumc"
    install -Dm644 /dev/stdin "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE" <<'LICEOF'
MIT License — see https://github.com/Ferrum-Language/Ferrum/blob/main/LICENSE
LICEOF
}
