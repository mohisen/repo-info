## `swipl:latest`

```console
$ docker pull swipl@sha256:33b7daed712d186abd65f95044802f4cf5d520bef2dc89b9c6fdbcd9c9114787
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `swipl:latest` - linux; amd64

```console
$ docker pull swipl@sha256:71c2484cc61800ab5cbf5bb95c533f24d24ca63ab687add196c21f6b16da778b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56228302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294706c05cdffd00e01012a3a5d77a9ebcbb4eba59539fbf09f636cb6c670bcd`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 13 Mar 2018 22:27:37 GMT
ADD file:e3250bb9848f956bdb43b205f1237df0d81a25088c95dbdeb20a1e2baf1d884f in / 
# Tue, 13 Mar 2018 22:27:37 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 23:24:00 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Wed, 14 Mar 2018 23:24:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libarchive13     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     { [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || apt-get install -y --no-install-recommends librocksdb4.5; } &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Mar 2018 23:27:41 GMT
RUN set -eux;     SWIPL_VER=7.7.10;     SWIPL_CHECKSUM=c2e01c55a696522b1dea0eb4da7bd9d398f36869af01b688f21246aaf55ef262;     BUILD_DEPS='make gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev';     dpkgArch="$(dpkg --print-architecture)";     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || BUILD_DEPS="$BUILD_DEPS librocksdb-dev";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget http://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     cd swipl-$SWIPL_VER;     sed -e '/PREFIX=$HOME/c\PREFIX=/usr'         -e '/# export DISABLE_PKGS/c\export DISABLE_PKGS="jpl xpce"'         -e 's/# *\(EXTRA.*--disable-libdirversion\)/\1/'            build.templ > build;     chmod u+x build; ./build;     mkdir -p /usr/lib/swipl/pack;     cd /usr/lib/swipl/pack;     rm -rf /tmp/src;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'space' ]; then (cd "$1"; ln -s configure.ac configure.in); fi;         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git a1d915d07933ece27ea5fd68f07c83d10583e7a0;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git 29eaee6fcdb6dce690ed187ef68b80ee94739412;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git 72838bbfa3976a83d19fb38bdae04378e30f4b0d;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 14 Mar 2018 23:27:41 GMT
ENV LANG=C.UTF-8
# Wed, 14 Mar 2018 23:27:41 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:2a72cbf407d67c7a7a76dd48e432091678e297140dce050ad5eccad918a9f8d6`  
		Last Modified: Tue, 13 Mar 2018 22:54:21 GMT  
		Size: 22.5 MB (22488979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f1d43940f2a1eb4ed0da6d952bf76008b32ced8a99d71f9d1ac25f9174358c`  
		Last Modified: Wed, 14 Mar 2018 23:37:28 GMT  
		Size: 26.3 MB (26259139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3ad5b2873934aa527f6e7b678c1b3323e2fc76d73fb490ea538b3838ac469`  
		Last Modified: Wed, 14 Mar 2018 23:37:26 GMT  
		Size: 7.5 MB (7480184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:latest` - linux; arm variant v7

```console
$ docker pull swipl@sha256:a0bed776bf4c92b6464f48e4eb8fa35f3fc73d1e1afe4280f842fb125cc7ee96
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48557536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a232a61985fc4ff9bdada23ef12c41f39a4ac9e6bef6567ca32857da4715d9`
-	Default Command: `["swipl"]`

```dockerfile
# Wed, 14 Mar 2018 12:33:12 GMT
ADD file:f766c04443a9148691357e97aad9ecafe1a8b4995a429d01337e669edeb93da2 in / 
# Wed, 14 Mar 2018 12:33:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:06:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Wed, 14 Mar 2018 13:06:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libarchive13     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     { [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || apt-get install -y --no-install-recommends librocksdb4.5; } &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Mar 2018 13:10:22 GMT
RUN set -eux;     SWIPL_VER=7.7.10;     SWIPL_CHECKSUM=c2e01c55a696522b1dea0eb4da7bd9d398f36869af01b688f21246aaf55ef262;     BUILD_DEPS='make gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev';     dpkgArch="$(dpkg --print-architecture)";     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || BUILD_DEPS="$BUILD_DEPS librocksdb-dev";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget http://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     cd swipl-$SWIPL_VER;     sed -e '/PREFIX=$HOME/c\PREFIX=/usr'         -e '/# export DISABLE_PKGS/c\export DISABLE_PKGS="jpl xpce"'         -e 's/# *\(EXTRA.*--disable-libdirversion\)/\1/'            build.templ > build;     chmod u+x build; ./build;     mkdir -p /usr/lib/swipl/pack;     cd /usr/lib/swipl/pack;     rm -rf /tmp/src;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'space' ]; then (cd "$1"; ln -s configure.ac configure.in); fi;         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git a1d915d07933ece27ea5fd68f07c83d10583e7a0;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git 29eaee6fcdb6dce690ed187ef68b80ee94739412;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git 72838bbfa3976a83d19fb38bdae04378e30f4b0d;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 14 Mar 2018 13:10:23 GMT
ENV LANG=C.UTF-8
# Wed, 14 Mar 2018 13:10:23 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:752dd0920056531abfaa5b01106ccd62d69cd92b84449b98f46b15b5b8495ac8`  
		Last Modified: Wed, 14 Mar 2018 12:45:14 GMT  
		Size: 19.3 MB (19277610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362e4c5c4293c0ee24221d715014d0c3459a3bea0cbc7398c750058c96e8ad3f`  
		Last Modified: Wed, 14 Mar 2018 13:10:59 GMT  
		Size: 22.7 MB (22683442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31733934f5b7e63a8fabd5196f1fceb8df7cc990610264cc63ce724c7b5b913b`  
		Last Modified: Wed, 14 Mar 2018 13:10:55 GMT  
		Size: 6.6 MB (6596484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
