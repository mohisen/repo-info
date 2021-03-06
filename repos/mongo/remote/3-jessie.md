## `mongo:3-jessie`

```console
$ docker pull mongo@sha256:d969194a7c4dcd817cae5dc726b1493547a3ad3f1b30f7f58857adc9ae6a4483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:fd85473bdcfad727d1d8d755a4879b7c7427a7fc84f50c92ab87508653469c6d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130528818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1317f8158fa35a66116d083d8c7e2c64720713b1ce90e2a1ec186e36a98984`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 06:29:43 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 14 Mar 2018 06:30:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Mar 2018 06:30:05 GMT
ENV GOSU_VERSION=1.10
# Wed, 14 Mar 2018 06:30:05 GMT
ENV JSYAML_VERSION=3.10.0
# Wed, 14 Mar 2018 06:30:31 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Wed, 14 Mar 2018 06:30:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 14 Mar 2018 06:32:28 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 14 Mar 2018 06:32:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 14 Mar 2018 06:32:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 14 Mar 2018 06:32:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 14 Mar 2018 06:32:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 14 Mar 2018 06:32:35 GMT
ENV MONGO_MAJOR=3.6
# Wed, 14 Mar 2018 06:32:35 GMT
ENV MONGO_VERSION=3.6.3
# Wed, 14 Mar 2018 06:32:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 14 Mar 2018 06:33:02 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 14 Mar 2018 06:33:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 14 Mar 2018 06:33:03 GMT
VOLUME [/data/db /data/configdb]
# Wed, 14 Mar 2018 06:33:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Wed, 14 Mar 2018 06:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Mar 2018 06:33:04 GMT
EXPOSE 27017/tcp
# Wed, 14 Mar 2018 06:33:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8b5b4e67a0c87e0946dcac28cc647a7e6c9331118dd0eef93747725d1dab7c`  
		Last Modified: Wed, 14 Mar 2018 07:02:24 GMT  
		Size: 2.1 KB (2094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87b29dbb5532144cd840d9b72eab4321de933a252e86cc472b61546f202c14e`  
		Last Modified: Wed, 14 Mar 2018 07:02:25 GMT  
		Size: 2.4 MB (2397877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908c259a6a99e48c455f1d2bf92c7174f7b4d3067f922fdf908d106ccd0d091c`  
		Last Modified: Wed, 14 Mar 2018 07:02:23 GMT  
		Size: 816.7 KB (816677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdec16e62a33da762a06b5a7e10ce995a2eb745168ec87d54aa8f5e52482617`  
		Last Modified: Wed, 14 Mar 2018 07:02:22 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e233c6c476cb9a3c3af96224851e2874771a736e19ef2c84b13c896e0d8044dc`  
		Last Modified: Wed, 14 Mar 2018 07:04:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671c302f3b4092b304b0bee534b3e911775ca626850456158211dddec06004d4`  
		Last Modified: Wed, 14 Mar 2018 07:04:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207ff3c88601bd15065d069fa544f5b73b6dc7e6fe0f1222f6d20506ac2fba8a`  
		Last Modified: Wed, 14 Mar 2018 07:04:26 GMT  
		Size: 97.2 MB (97184127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7998bea9fdf4dba81c93004e7641e5ef7ce64ec82aa24228152ba6f4ee2b3f`  
		Last Modified: Wed, 14 Mar 2018 07:04:08 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d605d67f267c15bedbf7720cbe79065e26004d4600c2ed87799dcfdd1e5331`  
		Last Modified: Wed, 14 Mar 2018 07:04:08 GMT  
		Size: 3.7 KB (3717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
