# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Babken Vardanyan <483ken@gmail.com>

_gemname=rubyzip
pkgname=ruby1.9-$_gemname
pkgver=1.1.6
pkgrel=1
pkgdesc='rubyzip is a ruby module for reading and writing zip files'
arch=(any)
url='http://github.com/rubyzip/rubyzip'
license=('BSD 2-Clause')
depends=(ruby1.9)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('eed01dd62083f4cf75a3cf34bcfb3413ac371ed0')

package() {
  local _gemdir="$(ruby-1.9 -e'puts Gem.default_dir')"
  gem-1.9 install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
