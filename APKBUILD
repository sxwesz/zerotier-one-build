# Maintainer: Your Name <your@email.com>
pkgname=zerotier-one
pkgver=1.12.2                      # 建议定期人工更新此版本号
pkgrel=0
pkgdesc="ZeroTier One - Global Area Networking"
url="https://www.zerotier.com"
arch="all"
license="GPL-3.0-or-later"
depends=""
makedepends="git g++ make linux-headers openssl-dev"
source="https://github.com/zerotier/ZeroTierOne/archive/refs/tags/$pkgver.tar.gz"

# 核心构建函数
build() {
    cd "$srcdir/ZeroTierOne-$pkgver"
    make
}

# 打包函数
package() {
    cd "$srcdir/ZeroTierOne-$pkgver"
    make DESTDIR="$pkgdir" install
}
