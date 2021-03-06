## `wordpress:php7.0-fpm-alpine`

```console
$ docker pull wordpress@sha256:5345f13cb89da3f77f61e73ea4d3d242d69050b90f6346878cc3d41cde43d087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `wordpress:php7.0-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:ae86385d3dd95a97cb013602a115785a2361f8df26c13fc2ee65488c912a3d6e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40077722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3842e274322d632d0672e6217c26ed37c465c8ae07a5de8a2ce75b14ec74f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Jan 2018 21:12:40 GMT
ADD file:69848cb51056edaf120230b6f218a79968ac797295c2cef6728332e1801357be in / 
# Tue, 09 Jan 2018 21:12:40 GMT
CMD ["/bin/sh"]
# Wed, 10 Jan 2018 03:00:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Jan 2018 03:00:28 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Jan 2018 03:00:35 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Jan 2018 03:00:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Jan 2018 03:00:36 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Wed, 10 Jan 2018 03:05:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Wed, 10 Jan 2018 03:05:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Wed, 10 Jan 2018 03:05:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Wed, 10 Jan 2018 03:05:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 10 Jan 2018 03:54:25 GMT
ENV GPG_KEYS=1A4E8B7277C42E53DBA9C7B9BCAA30EA9C0D5763 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Mon, 05 Mar 2018 23:08:26 GMT
ENV PHP_VERSION=7.0.28
# Mon, 05 Mar 2018 23:08:26 GMT
ENV PHP_URL=https://secure.php.net/get/php-7.0.28.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-7.0.28.tar.xz.asc/from/this/mirror
# Mon, 05 Mar 2018 23:08:26 GMT
ENV PHP_SHA256=e738ffce2c30bc0e84be9446af86bef0a0607d321f1a3d04bbfe2402fb5f6de0 PHP_MD5=
# Mon, 05 Mar 2018 23:09:25 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Mon, 05 Mar 2018 23:09:25 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Mon, 05 Mar 2018 23:13:04 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		coreutils 		curl-dev 		libedit-dev 		openssl-dev 		libxml2-dev 		sqlite-dev 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Mon, 05 Mar 2018 23:13:05 GMT
COPY multi:f9544e5c6b9d1d1292fca43464fe1e77b631547ac2baa8503de318853c0536d0 in /usr/local/bin/ 
# Mon, 05 Mar 2018 23:13:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 05 Mar 2018 23:13:06 GMT
WORKDIR /var/www/html
# Mon, 05 Mar 2018 23:13:06 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Mon, 05 Mar 2018 23:13:06 GMT
EXPOSE 9000/tcp
# Mon, 05 Mar 2018 23:13:07 GMT
CMD ["php-fpm"]
# Tue, 06 Mar 2018 04:06:52 GMT
RUN apk add --no-cache 		bash 		sed
# Tue, 06 Mar 2018 04:07:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Tue, 06 Mar 2018 04:07:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 06 Mar 2018 04:07:31 GMT
VOLUME [/var/www/html]
# Tue, 06 Mar 2018 04:07:31 GMT
ENV WORDPRESS_VERSION=4.9.4
# Tue, 06 Mar 2018 04:07:31 GMT
ENV WORDPRESS_SHA1=0e630bf940fd586b10e099cd9195b3e825fb194c
# Tue, 06 Mar 2018 04:07:33 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Tue, 06 Mar 2018 04:07:34 GMT
COPY file:3d3c99e98daa50fa9919315d4531e921f800fc011486bda46e9d6dcea82dd53c in /usr/local/bin/ 
# Tue, 06 Mar 2018 04:07:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Mar 2018 04:07:34 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:81033e7c1d6a5b44a94bb6b40033a6e589f50fd6b61578da6fc809e61f83898d`  
		Last Modified: Tue, 09 Jan 2018 21:15:04 GMT  
		Size: 2.4 MB (2387570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347280e4401ec27a2af6bcded9c9fe28c0acbe751f69f1d47c4fd6d2c82ba034`  
		Last Modified: Wed, 10 Jan 2018 04:40:03 GMT  
		Size: 1.3 MB (1324983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575b1e17046fe1c06043ae027f4599ed64f34196604a884d74c8942cdf71873e`  
		Last Modified: Wed, 10 Jan 2018 04:40:02 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26c263d6f029c4ccdfe4f8da176f53cbf3870d7d83f852d8b05ec3a606374d9`  
		Last Modified: Wed, 10 Jan 2018 04:40:00 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e153380334a5cd221ff87f0822f6e6ed41758b45e25d734ea7f57571ae2c817`  
		Last Modified: Tue, 06 Mar 2018 00:30:34 GMT  
		Size: 11.9 MB (11936674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1623f0523b592da5373b3517338615b1fca16e6995c6ec006db1d0da7a93c810`  
		Last Modified: Tue, 06 Mar 2018 00:30:31 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027c1d6bf29f3498694cff8f6dfe011dfb545f84c7979528a70293cdaf0633fa`  
		Last Modified: Tue, 06 Mar 2018 00:30:36 GMT  
		Size: 14.6 MB (14632474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd31fa41332b20406c4134f63b46e3a11ecfc40f318d693d0359e5ec4fb6b58`  
		Last Modified: Tue, 06 Mar 2018 00:30:31 GMT  
		Size: 2.2 KB (2168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c700a41c1a775ec2daea376ba016e7dd4f44ff1925eb69fc3f36f52d1bb24b5`  
		Last Modified: Tue, 06 Mar 2018 00:30:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b81e5ec64d9b8c33b60f002576076f241c9bf4af2569add41ffe0371bdf432`  
		Last Modified: Tue, 06 Mar 2018 00:30:30 GMT  
		Size: 7.7 KB (7658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91652b5fca6d11b2dcc76f31496c268372641acb04b16be14f26149acec754cd`  
		Last Modified: Tue, 06 Mar 2018 04:30:16 GMT  
		Size: 611.7 KB (611749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbf3bb26096dab28466b2f70e3ac0a2fe12d5150c5abf89208a242c7fc37d22`  
		Last Modified: Tue, 06 Mar 2018 04:30:16 GMT  
		Size: 746.4 KB (746400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f68ec1e7bd98861038f887f21a45600048b34ed5dcfe079bd2d113a14cf241`  
		Last Modified: Tue, 06 Mar 2018 04:30:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d828f119d6835d4025c75a0845d4613e4679297091084afdbaf0ef78c4a155f`  
		Last Modified: Tue, 06 Mar 2018 04:30:19 GMT  
		Size: 8.4 MB (8422292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd37f54ba730705f5aa1482b528f920415d82c7c903eeda1d9936dcc1226c2a`  
		Last Modified: Tue, 06 Mar 2018 04:30:16 GMT  
		Size: 3.3 KB (3348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
