# Maintainer: LINUX-GAMING.RU (tergoevm@gmail.com)

pkgname=portproton
pkgver=1.0
pkgrel=15
pkgdesc="Software for playing Microsoft Windows games and launchers"
arch=('x86_64')
url="https://linux-gaming.ru"
license=('MIT')
depends=('procps-ng' 'bash' 'icoutils' 'yad' 'wget' 'bubblewrap' 'zstd' 'cabextract' 'gzip'
         'bc' 'tar' 'openssl' 'desktop-file-utils' 'curl' 'dbus' 'freetype2' 'xdg-utils'
         'gdk-pixbuf2' 'ttf-font' 'zenity' 'nss' 'xorg-xrandr' 'lsof' 'mesa-utils'
         'vulkan-driver' 'vulkan-icd-loader' 'lib32-libgl' 'lib32-gcc-libs' 'vulkan-tools'
         'lib32-libx11' 'lib32-libxss' 'lib32-alsa-plugins' 'lib32-libgpg-error' 'lib32-freetype2'
         'lib32-nss' 'lib32-vulkan-driver' 'lib32-vulkan-icd-loader' 'lib32-openssl' 'lib32-mesa-utils')
optdepends=('gamemode: Support for Feral GameMode'
            'lib32-gamemode: 32-bit support for Feral GameMode')
source=("https://raw.githubusercontent.com/Castro-Fidel/PortWINE/master/portwine_install_script/PortProton_1.0"
        "$pkgname.desktop"
        "$pkgname.svg"
        "$pkgname.metainfo.xml"
        "LICENSE")
sha256sums=('6fa73e20bf180ffa8b252d7d50dc43fcf62eed6caf8867e7a5bcf445daa6dabe'
            '17d2c7bc99707a88ec13422ff40f33004c8a41bf945143122d5ee0f6a3be3bce'
            'df2850787a0777bfd446bed40c6c2bcd6ce5636a241dfe08a6a915f151b20fd4'
            'c7889e20b1fa13c17327681b5f637df84c4019f95673e4bd168dceba31cea599'
            '65d12e4e0be4dd5e58324593563c8c79af42876d63f51225364b968117c6ff4f')

package() {
  install -Dm755 "PortProton_$pkgver" "$pkgdir/usr/bin/$pkgname"
  install -Dm644 "$pkgname.desktop" -t "$pkgdir/usr/share/applications/"
  install -Dm644 "$pkgname.svg" -t "$pkgdir/usr/share/icons/hicolor/scalable/apps/"
  install -Dm644 "$pkgname.metainfo.xml" -t "$pkgdir/usr/share/metainfo/"
  install -Dm644 LICENSE -t "$pkgdir/usr/share/licenses/$pkgname/"
}
