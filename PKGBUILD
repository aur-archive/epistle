# Maintainer: Sarkasper <echo a2FzcGVyLm1lbnRlbkBnbXguY29tCg==|base64 -d>
# Contributor: Logan Allen <loganfynne at gmail dot com>
pkgname=epistle
pkgver=0.11.0
pkgrel=19
pkgdesc='Lightweight Social Email Client - Email, Twitter, and Facebook Support'
arch=('any')
url="https://bitbucket.org/loganfynne/epistle"
license=('GPL')
makedepends=('python2-distribute')
depends=('python2' 'pygtk' 'pywebkitgtk' 'python2-tweepy-git')
source=(https://bitbucket.org/loganfynne/epistle/get/1b3185e0153d.tar.bz2)
md5sums=('14be38fd36bfbcc9343e411b0c018838')

package() {
  mkdir -p ${pkgdir}/usr/share/applications
  mkdir -p ${pkgdir}/usr/lib/epistle
  mkdir -p ${pkgdir}/usr/bin
  cp -r */* ${pkgdir}/usr/lib/epistle/
  chmod +x ${pkgdir}/usr/lib/epistle/epistle.py
  cp */epistle ${pkgdir}/usr/bin/
  chmod +x ${pkgdir}/usr/bin/epistle
  cp */epistle.desktop ${pkgdir}/usr/share/applications/
}
