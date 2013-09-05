mod_ranged
==========
Apache module for [libcrange](https://github.com/boinger/libcrange)

## Prereqs (to build)
    apr
    apr-devel
    apr-util
    apr-util-devel
    db4-cxx
    db4-devel
    expat-devel
    flex
    httpd
    httpd-devel
    httpd-tools
    [libcrange](https://github.com/boinger/libcrange)
    libyaml
    pcre
    pcre-devel

    perl
    perl-ExtUtils-ParseXS
    perl-ExtUtils-MakeMaker
    perl-ExtUtils-Embed
    perl-Module-Pluggable
    perl-Pod-Escapes
    perl-Pod-Simple
    perl-Test-Harness
    perl-devel
    perl-libs
    perl-version

    sqlite-devel
    zlib
    zlib-devel

    perl-Test-Simple
    perl-libwww-perl

## RPM build

From the libcrange directory, assuming a standard homedir-based `rpmdev-setuptree` setup
```bash
ln -s `pwd`/mod_ranged.spec ~/rpmbuild/SPECS
tar cvfz ~/rpmbuild/SOURCES/mod_ranged-latest.tar.gz source root
rpmbuild -ba mod_ranged.spec
```