## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:382738a23eafc1c891388e1b139326748a4c52f838a0d9867ebd1b8dbc619077
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	windows version 10.0.14393.2125; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:4ed3a8047c153adaf5029873c4e272c8a372ba645546b865ed6db6c0642144b8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3807912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19a3b12418d33d30e14dbaddd66da82c56a99b5243dcbff5f161f5e0037ceb68`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Mar 2018 20:55:57 GMT
COPY file:b2a7a3cb2cdb8a50e1396d46c0abd2d6e78521b77aa1c9ebcb274599b68e343a in /nats-streaming-server 
# Fri, 16 Mar 2018 20:55:57 GMT
EXPOSE 4222/tcp 8222/tcp
# Fri, 16 Mar 2018 20:55:57 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Mar 2018 20:55:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9a9204bf6dd332233debc2bfe8fbf4c773e0a7aafd451bd1ca3a34dca234d3a2`  
		Last Modified: Fri, 16 Mar 2018 20:56:22 GMT  
		Size: 3.8 MB (3807912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:66ccae6d73184c1ca34bab4d3bbee608ec17f019eec847c29a210055aea9e8a1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3566357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e7046b456b34417f7b7ba41e4662215d5e5b0c0f434b7eaf3c2ab7faff5f20`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Mar 2018 23:27:45 GMT
COPY file:a9b9004c78701f1dc8a89548244aba9ac628fe569de11ba648d8aecfa0ea91b2 in /nats-streaming-server 
# Fri, 16 Mar 2018 23:27:45 GMT
EXPOSE 4222/tcp 8222/tcp
# Fri, 16 Mar 2018 23:27:46 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Mar 2018 23:27:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf7c12c2515e56ab58b16381c8d0d51e28e5090e9d033bc3ae01c5f26253812`  
		Last Modified: Fri, 16 Mar 2018 23:28:06 GMT  
		Size: 3.6 MB (3566357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.14393.2125; amd64

```console
$ docker pull nats-streaming@sha256:8fde1bb8c8a80f486493bdc0393793e480046a8732630c3d0f7d84df54a1d476
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.6 MB (412550447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea852e8aa9ddd5b45a3ee7d9184a5eb91ba17bc41ff3e1d7b60b9d50301f1c29`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 13 Dec 2016 10:47:17 GMT
RUN Apply image 10.0.14393.0
# Tue, 13 Mar 2018 00:52:57 GMT
RUN Install update 10.0.14393.2125
# Tue, 13 Mar 2018 23:39:00 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Mar 2018 22:21:51 GMT
RUN cmd /S /C #(nop) WORKDIR C:\nats-streaming-server
# Fri, 16 Mar 2018 22:22:02 GMT
RUN cmd /S /C #(nop) COPY file:89353859e56ad4eec04e662f40cbb2c64630a73e0df63e4deb487a48c0fc0d44 in nats-streaming-server.exe 
# Fri, 16 Mar 2018 22:22:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222/tcp 8222/tcp
# Fri, 16 Mar 2018 22:22:05 GMT
RUN cmd /S /C #(nop)  CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bce2fbc256ea437a87dadac2f69aabd25bed4f56255549090056c1131fad0277`  
		Last Modified: Tue, 13 Dec 2016 10:47:17 GMT  
		Size: 252.7 MB (252691002 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b557cd80a9856d964887c4ea407b85fca10ce6aaa539984be9dd3570c60fd66`  
		Last Modified: Tue, 13 Mar 2018 00:52:57 GMT  
		Size: 156.0 MB (156003306 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cd6679018c86917df531ece3d8500b5dfaccb8b79ba313225e6b0f40be5f9f9d`  
		Last Modified: Tue, 13 Mar 2018 23:39:33 GMT  
		Size: 915.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6214d441b14aa67647b0d3366fbf1d6a802b7457ca11fe0f50ed57147e2a4e87`  
		Last Modified: Wed, 14 Mar 2018 22:22:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2576b109caf4fa55c9334c599c33570a73e9a6f81667abc72ef8fd626e4fa9c`  
		Last Modified: Fri, 16 Mar 2018 22:22:26 GMT  
		Size: 3.9 MB (3852160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602742b0f911ca83b400ef384140adda4519892971d87d7a4681e2971250c36a`  
		Last Modified: Fri, 16 Mar 2018 22:22:24 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156247ead4b4b7fce1f6d4e65d5bdd34e2f44ccca9e61c6e75e653caeea689e`  
		Last Modified: Fri, 16 Mar 2018 22:22:24 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
