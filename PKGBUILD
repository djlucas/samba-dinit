# Maintainer: Muhammad Herdiansyah <koni@artixlinux.org>

pkgname=samba-dinit
pkgver=20260222
pkgrel=1
pkgdesc="dinit service scripts for samba"
arch=('any')
url="https://artixlinux.org"
license=('BSD')
groups=('dinit-world')
depends=('samba' 'dinit')
conflicts=('init-samba')
provides=('init-samba')
source=("smbd"
        "nmbd"
        "samba"
        "samba-pre"
        "winbindd")
sha256sums=('e1b4f4586e08d1043cd6707c1d02db1c815b62d692ca8d975352d55a36259332'
            '21fccdb056b80970f4306482b0c26e51ab0e0e298ac7290054b41f527f5e3df3'
            '376628b46d2145bed6cf6e3db1b05c19032992b3434984bcf68eaedd04046b56'
            'e3fd62e239d6be4513dbbf3a50c7bc55bc30760e3679d23c340ede0cc7f44ffd'
            '1177ca4b1cc66a57f178f289986cc0e3c66407ebb8253195aaa18781fa800065')

package() {
    install -Dm644 smbd      "$pkgdir/etc/dinit.d/smbd"
    install -Dm644 nmbd      "$pkgdir/etc/dinit.d/nmbd"
    install -Dm644 samba     "$pkgdir/etc/dinit.d/samba"
    install -Dm644 samba-pre "$pkgdir/etc/dinit.d/samba-pre"
    install -Dm644 winbindd  "$pkgdir/etc/dinit.d/winbindd"
}
