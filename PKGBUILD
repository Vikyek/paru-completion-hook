pkgname=paru-completion-hook
pkgver=1.0.0
pkgrel=1
pkgdesc="Pacman hook and systemd path unit to automatically update the paru completion cache"
arch=('any')
url="https://github.com/v/paru-completion-hook"
license=('GPL')
depends=('paru' 'bash')
install=paru-completion-hook.install
source=(
    "paru-completion-update"
    "paru-completion-update.hook"
    "paru-completion-update.path"
    "paru-completion-update.service"
)
sha256sums=('c1398967c4d0591f7cd4e1973b0ca9fe95aea33b925ad18b410590f7327ac38f'
            '82006c2834506fe87ae43f18bdecfe713952ee13fac403fdba3fe9250ec840ed'
            '8ab053fa324e5cbd5d635895bd500ffaebeafbe11fa0c7704329acaa3d6dabd9'
            'aee25152324bbe9aa467f7e3274d21eaa53fb201dddea98baa81c7832fce1565')

package() {
    # Install update script
    install -Dm755 "${srcdir}/paru-completion-update" "${pkgdir}/usr/bin/paru-completion-update"

    # Install pacman hook
    install -Dm644 "${srcdir}/paru-completion-update.hook" "${pkgdir}/usr/share/libalpm/hooks/paru-completion-update.hook"

    # Install systemd path and service units
    install -Dm644 "${srcdir}/paru-completion-update.path" "${pkgdir}/usr/lib/systemd/system/paru-completion-update.path"
    install -Dm644 "${srcdir}/paru-completion-update.service" "${pkgdir}/usr/lib/systemd/system/paru-completion-update.service"
}
