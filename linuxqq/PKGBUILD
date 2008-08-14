# Contributor: leafduo <leafduo@gmail.com>
pkgname=linuxqq
pkgver=1.0_Preview1
pkgrel=2
pkgdesc="QQ for Linux 1.0 Preview"
url="http://www.qq.com/"
license=("copyrighted")
depends=('gtk2>=2.10')
arch=(i686)
makedepends=('tar')
source=(http://dl_dir.qq.com/linuxqq/linuxqq_1.0-Preview1_i386.deb)
md5sums=('cf95014386fb69981ba30444b06aedb5')
build() {
    cd $startdir/src/
    ar vx linuxqq_1.0-Preview1_i386.deb
    tar xfz data.tar.gz
    chmod 0755 $startdir/src/usr/bin/QQ $startdir/src/usr/share/apps/Tencent/QQ/*
    cp -a $startdir/src/usr $startdir/pkg
    ln -s /usr/bin/QQ $startdir/pkg/usr/bin/qq
}
