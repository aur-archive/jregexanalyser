# Maintainer: Baobab <eternal.baobab@gmail.com>

pkgname=jregexanalyser
pkgver=1.4.0
pkgrel=1
pkgdesc="Interactive tool to write, test, debug, analyse and profile regular expressions"
arch=('any')
url="http://jregexanalyser.schwebke.com"
license=('GPL')
depends=('java-runtime')
source=("http://jregexanalyser.schwebke.com/jregexanalyser/jRegExAnalyser-1_4_0.zip"
        "jregexanalyser.sh")
md5sums=('befcfd8e1b0a6b19970f745a2933ebad'
         '283025b0c873c4d201e3753408fcacfb')

build() {
    install -d $pkgdir/usr/share/java/$pkgname
    install -m644 $srcdir/jRegExAnalyser-1_4_0/jRegExAnalyser.jar $pkgdir/usr/share/java/$pkgname
    install -m644 $srcdir/jRegExAnalyser-1_4_0/lib/jnlp.jar $pkgdir/usr/share/java/$pkgname
    install -D -m755 $srcdir/jregexanalyser.sh $pkgdir/usr/bin/jregexanalyser
    install -D -m644 $srcdir/jRegExAnalyser-1_4_0/jregexanalyser.desktop $pkgdir/usr/share/applications/jregexanalyser.desktop
    install -D -m644 $srcdir/jRegExAnalyser-1_4_0/icon.png $pkgdir/usr/share/pixmaps/jregexanalyser.png    
    install -D -m644 $srcdir/jRegExAnalyser-1_4_0/readme.txt $pkgdir/usr/share/doc/$pkgname/readme.txt
    cp -r $srcdir/jRegExAnalyser-1_4_0/webdoc $pkgdir/usr/share/doc/$pkgname
}
