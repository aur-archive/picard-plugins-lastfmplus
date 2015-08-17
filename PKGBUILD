# Contributor: Johannes Dewender  arch at JonnyJD dot net
pkgname=picard-plugins-lastfmplus
pkgver=1.0
pkgrel=1
pkgdesc="LastFMPlus Plugin for MusicBrainz Picard"
arch=('any')
url="http://wiki.musicbrainz.org/Picard_Documentation/Plugins/Lastfmplus"
license=('GPL')
depends=('picard')
# temporary source, file is only on mediafire:
# http://www.mediafire.com/?qlso9gc8c75aq5a
source=(http://kraehen.org/tmp/lastfmplus-0.13.zip)
md5sums=('b19395bc1a0fe6a937c1350baf5c2e0b')

build() {
  plugindir=${pkgdir}/usr/lib/python2.7/site-packages/picard/plugins
  cd "$srcdir"/lastfmplus
  mkdir -p $plugindir/lastfmplus
  chmod a-x __init__.py ui_options_lastfm.py
  cp __init__.py ui_options_lastfm.py $plugindir/lastfmplus
}

# vim:set ts=2 sw=2 et:
