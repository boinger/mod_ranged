mod_ranged
==========
Apache module for [libcrange](https://github.com/boinger/libcrange)

## Prereqs
### To build
    apr-util-devel
    httpd-devel
    pcre-devel
    sqlite-devel
    zlib-devel

### To run
    flex
    libyaml
    perl-ExtUtils-MakeMaker
    perl-ExtUtils-Embed
    perl-Test-Simple
    perl-libwww-perl
    pcre
    zlib

## RPM build

From the libcrange directory, assuming a standard homedir-based `rpmdev-setuptree` setup
```bash
ln -s `pwd`/mod_ranged.spec ~/rpmbuild/SPECS
tar cvfz ~/rpmbuild/SOURCES/mod_ranged-latest.tar.gz source root
cd ~/rpmbuild/SPECS
rpmbuild -ba mod_ranged.spec
```