<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mono`

-	[`mono:4`](#mono4)
-	[`mono:4.8`](#mono48)
-	[`mono:4.8.0`](#mono480)
-	[`mono:4.8.0.524`](#mono480524)
-	[`mono:5`](#mono5)
-	[`mono:5.4`](#mono54)
-	[`mono:5.4.1`](#mono541)
-	[`mono:5.4.1.6`](#mono5416)
-	[`mono:5.4.1.6-slim`](#mono5416-slim)
-	[`mono:5.4.1-slim`](#mono541-slim)
-	[`mono:5.4-slim`](#mono54-slim)
-	[`mono:5.8`](#mono58)
-	[`mono:5.8.0`](#mono580)
-	[`mono:5.8.0.127`](#mono580127)
-	[`mono:5.8.0.127-slim`](#mono580127-slim)
-	[`mono:5.8.0-slim`](#mono580-slim)
-	[`mono:5.8-slim`](#mono58-slim)
-	[`mono:5-slim`](#mono5-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:4`

```console
$ docker pull mono@sha256:e759334e7a01f53db2f03067a17cbce0b17e56e4b5e648502d94d4814eed26e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4` - linux; amd64

```console
$ docker pull mono@sha256:24ca2f769ff50c3bf26fb29b3996fcbae921712dd2864d986763fcfc74c4d53a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153044010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21395e539446961c8c79889c83213ec8fa692960d3bb82e5b28e3d5e585611f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 22:31:05 GMT
ADD file:fc9ba15f087e646a9d3b72e742eb1233132a118ecfa998e2497b724f3ff84061 in / 
# Tue, 13 Mar 2018 22:31:06 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:25:16 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Wed, 14 Mar 2018 07:25:16 GMT
ENV MONO_VERSION=4.8.0.524
# Wed, 14 Mar 2018 07:25:27 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Mar 2018 07:25:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:29:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4269eaa217cc08668f088a9719d43c993c4644a73eda4eb55921f031a4311060`  
		Last Modified: Tue, 13 Mar 2018 22:58:14 GMT  
		Size: 38.1 MB (38111490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6147e46c1801b7e5f38122640067362c4ce1856790fe765e5efe9c177a6d799f`  
		Last Modified: Wed, 14 Mar 2018 07:39:40 GMT  
		Size: 7.8 MB (7755499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2696f2583834864fdb612decc9519d666b07379b32f82265b362f7b6afbe37`  
		Last Modified: Wed, 14 Mar 2018 07:39:39 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db2610465588aa2981eb82d742b84dcf38afe00210a711c8503d7ec32ebbcc`  
		Last Modified: Wed, 14 Mar 2018 07:40:05 GMT  
		Size: 107.1 MB (107147113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4` - linux; arm variant v7

```console
$ docker pull mono@sha256:c342c7ceeb0ef7ad549cd05f28f2af9b13c4cd80b1aabdd1a807785dfa1b0e83
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138944851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b55a944b76eecfa8b409ff92f9331c59604b352c62a0048b1aaf2ebe6a6cb7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:36:11 GMT
ADD file:9db26feeeebe82707411c8b6a09f22ba8e33fdd8bdf1e1cb3fd179cfc09b850e in / 
# Tue, 12 Dec 2017 13:36:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:42:42 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Tue, 12 Dec 2017 14:42:42 GMT
ENV MONO_VERSION=4.8.0.524
# Tue, 12 Dec 2017 14:42:57 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:42:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 12 Dec 2017 14:44:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:dd70000a68c40049fa024e9ebecc22bcd8a32b0fb098e9f3edafdbfc872054b4`  
		Last Modified: Tue, 12 Dec 2017 13:47:59 GMT  
		Size: 35.7 MB (35661805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bac5781424193c9527b5bfa5c06eb028e0eca16516cd058511653a01b0b7dd`  
		Last Modified: Tue, 12 Dec 2017 14:50:53 GMT  
		Size: 7.2 MB (7185300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567cfe4d52b53ccc0a2131014faead07f90583cded9e13a802fd7ba39c4bbc67`  
		Last Modified: Tue, 12 Dec 2017 14:50:52 GMT  
		Size: 29.9 KB (29910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e170876330ebd96f24bce96ea82eb2241088331591e17d2b66fb8b7e6a0c3c`  
		Last Modified: Tue, 12 Dec 2017 14:51:26 GMT  
		Size: 96.1 MB (96067836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4` - linux; 386

```console
$ docker pull mono@sha256:43927f1c0933c579c97349e544890626770ab1aa448d8d081d3cdd3735342060
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153059206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ef815aafcd5e327a9fc3d4d98037b2c4e5663014cc1fa58a9e2c11d040ff96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 20:34:29 GMT
ADD file:b269dd25aa5a2b39f29e341376ca9f2b8aded8f1327c01024b96a2eaa5c3a142 in / 
# Thu, 15 Feb 2018 20:34:29 GMT
CMD ["bash"]
# Fri, 16 Feb 2018 11:39:49 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Fri, 16 Feb 2018 11:39:50 GMT
ENV MONO_VERSION=4.8.0.524
# Fri, 16 Feb 2018 11:40:06 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Fri, 16 Feb 2018 11:40:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Fri, 16 Feb 2018 11:41:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f10fe2356c6af971fa6e4de75405f5f2c0a1b4dd473c5da5cca0dc476bf491f8`  
		Last Modified: Thu, 15 Feb 2018 01:29:03 GMT  
		Size: 37.4 MB (37439124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e617752d4f547c030861e5d17fe22d2a1a97a5719106a706bb9087aab6788984`  
		Last Modified: Fri, 16 Feb 2018 12:04:35 GMT  
		Size: 9.6 MB (9607507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0c5d1b4144aae8c52ba8fd6fbb632e1e4bb1ad1938e34fcf51b791efc2937b`  
		Last Modified: Fri, 16 Feb 2018 12:04:31 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8323e44890fa0ebf489071f9912d8e2339baab4ba4395fd35a51b71c2d63825`  
		Last Modified: Fri, 16 Feb 2018 12:05:14 GMT  
		Size: 106.0 MB (105982667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:4.8`

```console
$ docker pull mono@sha256:e759334e7a01f53db2f03067a17cbce0b17e56e4b5e648502d94d4814eed26e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4.8` - linux; amd64

```console
$ docker pull mono@sha256:24ca2f769ff50c3bf26fb29b3996fcbae921712dd2864d986763fcfc74c4d53a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153044010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21395e539446961c8c79889c83213ec8fa692960d3bb82e5b28e3d5e585611f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 22:31:05 GMT
ADD file:fc9ba15f087e646a9d3b72e742eb1233132a118ecfa998e2497b724f3ff84061 in / 
# Tue, 13 Mar 2018 22:31:06 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:25:16 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Wed, 14 Mar 2018 07:25:16 GMT
ENV MONO_VERSION=4.8.0.524
# Wed, 14 Mar 2018 07:25:27 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Mar 2018 07:25:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:29:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4269eaa217cc08668f088a9719d43c993c4644a73eda4eb55921f031a4311060`  
		Last Modified: Tue, 13 Mar 2018 22:58:14 GMT  
		Size: 38.1 MB (38111490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6147e46c1801b7e5f38122640067362c4ce1856790fe765e5efe9c177a6d799f`  
		Last Modified: Wed, 14 Mar 2018 07:39:40 GMT  
		Size: 7.8 MB (7755499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2696f2583834864fdb612decc9519d666b07379b32f82265b362f7b6afbe37`  
		Last Modified: Wed, 14 Mar 2018 07:39:39 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db2610465588aa2981eb82d742b84dcf38afe00210a711c8503d7ec32ebbcc`  
		Last Modified: Wed, 14 Mar 2018 07:40:05 GMT  
		Size: 107.1 MB (107147113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8` - linux; arm variant v7

```console
$ docker pull mono@sha256:c342c7ceeb0ef7ad549cd05f28f2af9b13c4cd80b1aabdd1a807785dfa1b0e83
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138944851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b55a944b76eecfa8b409ff92f9331c59604b352c62a0048b1aaf2ebe6a6cb7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:36:11 GMT
ADD file:9db26feeeebe82707411c8b6a09f22ba8e33fdd8bdf1e1cb3fd179cfc09b850e in / 
# Tue, 12 Dec 2017 13:36:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:42:42 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Tue, 12 Dec 2017 14:42:42 GMT
ENV MONO_VERSION=4.8.0.524
# Tue, 12 Dec 2017 14:42:57 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:42:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 12 Dec 2017 14:44:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:dd70000a68c40049fa024e9ebecc22bcd8a32b0fb098e9f3edafdbfc872054b4`  
		Last Modified: Tue, 12 Dec 2017 13:47:59 GMT  
		Size: 35.7 MB (35661805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bac5781424193c9527b5bfa5c06eb028e0eca16516cd058511653a01b0b7dd`  
		Last Modified: Tue, 12 Dec 2017 14:50:53 GMT  
		Size: 7.2 MB (7185300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567cfe4d52b53ccc0a2131014faead07f90583cded9e13a802fd7ba39c4bbc67`  
		Last Modified: Tue, 12 Dec 2017 14:50:52 GMT  
		Size: 29.9 KB (29910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e170876330ebd96f24bce96ea82eb2241088331591e17d2b66fb8b7e6a0c3c`  
		Last Modified: Tue, 12 Dec 2017 14:51:26 GMT  
		Size: 96.1 MB (96067836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8` - linux; 386

```console
$ docker pull mono@sha256:43927f1c0933c579c97349e544890626770ab1aa448d8d081d3cdd3735342060
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153059206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ef815aafcd5e327a9fc3d4d98037b2c4e5663014cc1fa58a9e2c11d040ff96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 20:34:29 GMT
ADD file:b269dd25aa5a2b39f29e341376ca9f2b8aded8f1327c01024b96a2eaa5c3a142 in / 
# Thu, 15 Feb 2018 20:34:29 GMT
CMD ["bash"]
# Fri, 16 Feb 2018 11:39:49 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Fri, 16 Feb 2018 11:39:50 GMT
ENV MONO_VERSION=4.8.0.524
# Fri, 16 Feb 2018 11:40:06 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Fri, 16 Feb 2018 11:40:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Fri, 16 Feb 2018 11:41:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f10fe2356c6af971fa6e4de75405f5f2c0a1b4dd473c5da5cca0dc476bf491f8`  
		Last Modified: Thu, 15 Feb 2018 01:29:03 GMT  
		Size: 37.4 MB (37439124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e617752d4f547c030861e5d17fe22d2a1a97a5719106a706bb9087aab6788984`  
		Last Modified: Fri, 16 Feb 2018 12:04:35 GMT  
		Size: 9.6 MB (9607507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0c5d1b4144aae8c52ba8fd6fbb632e1e4bb1ad1938e34fcf51b791efc2937b`  
		Last Modified: Fri, 16 Feb 2018 12:04:31 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8323e44890fa0ebf489071f9912d8e2339baab4ba4395fd35a51b71c2d63825`  
		Last Modified: Fri, 16 Feb 2018 12:05:14 GMT  
		Size: 106.0 MB (105982667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:4.8.0`

```console
$ docker pull mono@sha256:e759334e7a01f53db2f03067a17cbce0b17e56e4b5e648502d94d4814eed26e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4.8.0` - linux; amd64

```console
$ docker pull mono@sha256:24ca2f769ff50c3bf26fb29b3996fcbae921712dd2864d986763fcfc74c4d53a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153044010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21395e539446961c8c79889c83213ec8fa692960d3bb82e5b28e3d5e585611f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 22:31:05 GMT
ADD file:fc9ba15f087e646a9d3b72e742eb1233132a118ecfa998e2497b724f3ff84061 in / 
# Tue, 13 Mar 2018 22:31:06 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:25:16 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Wed, 14 Mar 2018 07:25:16 GMT
ENV MONO_VERSION=4.8.0.524
# Wed, 14 Mar 2018 07:25:27 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Mar 2018 07:25:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:29:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4269eaa217cc08668f088a9719d43c993c4644a73eda4eb55921f031a4311060`  
		Last Modified: Tue, 13 Mar 2018 22:58:14 GMT  
		Size: 38.1 MB (38111490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6147e46c1801b7e5f38122640067362c4ce1856790fe765e5efe9c177a6d799f`  
		Last Modified: Wed, 14 Mar 2018 07:39:40 GMT  
		Size: 7.8 MB (7755499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2696f2583834864fdb612decc9519d666b07379b32f82265b362f7b6afbe37`  
		Last Modified: Wed, 14 Mar 2018 07:39:39 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db2610465588aa2981eb82d742b84dcf38afe00210a711c8503d7ec32ebbcc`  
		Last Modified: Wed, 14 Mar 2018 07:40:05 GMT  
		Size: 107.1 MB (107147113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:c342c7ceeb0ef7ad549cd05f28f2af9b13c4cd80b1aabdd1a807785dfa1b0e83
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138944851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b55a944b76eecfa8b409ff92f9331c59604b352c62a0048b1aaf2ebe6a6cb7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:36:11 GMT
ADD file:9db26feeeebe82707411c8b6a09f22ba8e33fdd8bdf1e1cb3fd179cfc09b850e in / 
# Tue, 12 Dec 2017 13:36:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:42:42 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Tue, 12 Dec 2017 14:42:42 GMT
ENV MONO_VERSION=4.8.0.524
# Tue, 12 Dec 2017 14:42:57 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:42:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 12 Dec 2017 14:44:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:dd70000a68c40049fa024e9ebecc22bcd8a32b0fb098e9f3edafdbfc872054b4`  
		Last Modified: Tue, 12 Dec 2017 13:47:59 GMT  
		Size: 35.7 MB (35661805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bac5781424193c9527b5bfa5c06eb028e0eca16516cd058511653a01b0b7dd`  
		Last Modified: Tue, 12 Dec 2017 14:50:53 GMT  
		Size: 7.2 MB (7185300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567cfe4d52b53ccc0a2131014faead07f90583cded9e13a802fd7ba39c4bbc67`  
		Last Modified: Tue, 12 Dec 2017 14:50:52 GMT  
		Size: 29.9 KB (29910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e170876330ebd96f24bce96ea82eb2241088331591e17d2b66fb8b7e6a0c3c`  
		Last Modified: Tue, 12 Dec 2017 14:51:26 GMT  
		Size: 96.1 MB (96067836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0` - linux; 386

```console
$ docker pull mono@sha256:43927f1c0933c579c97349e544890626770ab1aa448d8d081d3cdd3735342060
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153059206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ef815aafcd5e327a9fc3d4d98037b2c4e5663014cc1fa58a9e2c11d040ff96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 20:34:29 GMT
ADD file:b269dd25aa5a2b39f29e341376ca9f2b8aded8f1327c01024b96a2eaa5c3a142 in / 
# Thu, 15 Feb 2018 20:34:29 GMT
CMD ["bash"]
# Fri, 16 Feb 2018 11:39:49 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Fri, 16 Feb 2018 11:39:50 GMT
ENV MONO_VERSION=4.8.0.524
# Fri, 16 Feb 2018 11:40:06 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Fri, 16 Feb 2018 11:40:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Fri, 16 Feb 2018 11:41:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f10fe2356c6af971fa6e4de75405f5f2c0a1b4dd473c5da5cca0dc476bf491f8`  
		Last Modified: Thu, 15 Feb 2018 01:29:03 GMT  
		Size: 37.4 MB (37439124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e617752d4f547c030861e5d17fe22d2a1a97a5719106a706bb9087aab6788984`  
		Last Modified: Fri, 16 Feb 2018 12:04:35 GMT  
		Size: 9.6 MB (9607507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0c5d1b4144aae8c52ba8fd6fbb632e1e4bb1ad1938e34fcf51b791efc2937b`  
		Last Modified: Fri, 16 Feb 2018 12:04:31 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8323e44890fa0ebf489071f9912d8e2339baab4ba4395fd35a51b71c2d63825`  
		Last Modified: Fri, 16 Feb 2018 12:05:14 GMT  
		Size: 106.0 MB (105982667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:4.8.0.524`

```console
$ docker pull mono@sha256:e759334e7a01f53db2f03067a17cbce0b17e56e4b5e648502d94d4814eed26e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4.8.0.524` - linux; amd64

```console
$ docker pull mono@sha256:24ca2f769ff50c3bf26fb29b3996fcbae921712dd2864d986763fcfc74c4d53a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153044010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21395e539446961c8c79889c83213ec8fa692960d3bb82e5b28e3d5e585611f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 22:31:05 GMT
ADD file:fc9ba15f087e646a9d3b72e742eb1233132a118ecfa998e2497b724f3ff84061 in / 
# Tue, 13 Mar 2018 22:31:06 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:25:16 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Wed, 14 Mar 2018 07:25:16 GMT
ENV MONO_VERSION=4.8.0.524
# Wed, 14 Mar 2018 07:25:27 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Mar 2018 07:25:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:29:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4269eaa217cc08668f088a9719d43c993c4644a73eda4eb55921f031a4311060`  
		Last Modified: Tue, 13 Mar 2018 22:58:14 GMT  
		Size: 38.1 MB (38111490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6147e46c1801b7e5f38122640067362c4ce1856790fe765e5efe9c177a6d799f`  
		Last Modified: Wed, 14 Mar 2018 07:39:40 GMT  
		Size: 7.8 MB (7755499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2696f2583834864fdb612decc9519d666b07379b32f82265b362f7b6afbe37`  
		Last Modified: Wed, 14 Mar 2018 07:39:39 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db2610465588aa2981eb82d742b84dcf38afe00210a711c8503d7ec32ebbcc`  
		Last Modified: Wed, 14 Mar 2018 07:40:05 GMT  
		Size: 107.1 MB (107147113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0.524` - linux; arm variant v7

```console
$ docker pull mono@sha256:c342c7ceeb0ef7ad549cd05f28f2af9b13c4cd80b1aabdd1a807785dfa1b0e83
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138944851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b55a944b76eecfa8b409ff92f9331c59604b352c62a0048b1aaf2ebe6a6cb7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:36:11 GMT
ADD file:9db26feeeebe82707411c8b6a09f22ba8e33fdd8bdf1e1cb3fd179cfc09b850e in / 
# Tue, 12 Dec 2017 13:36:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:42:42 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Tue, 12 Dec 2017 14:42:42 GMT
ENV MONO_VERSION=4.8.0.524
# Tue, 12 Dec 2017 14:42:57 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:42:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 12 Dec 2017 14:44:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:dd70000a68c40049fa024e9ebecc22bcd8a32b0fb098e9f3edafdbfc872054b4`  
		Last Modified: Tue, 12 Dec 2017 13:47:59 GMT  
		Size: 35.7 MB (35661805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bac5781424193c9527b5bfa5c06eb028e0eca16516cd058511653a01b0b7dd`  
		Last Modified: Tue, 12 Dec 2017 14:50:53 GMT  
		Size: 7.2 MB (7185300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567cfe4d52b53ccc0a2131014faead07f90583cded9e13a802fd7ba39c4bbc67`  
		Last Modified: Tue, 12 Dec 2017 14:50:52 GMT  
		Size: 29.9 KB (29910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e170876330ebd96f24bce96ea82eb2241088331591e17d2b66fb8b7e6a0c3c`  
		Last Modified: Tue, 12 Dec 2017 14:51:26 GMT  
		Size: 96.1 MB (96067836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0.524` - linux; 386

```console
$ docker pull mono@sha256:43927f1c0933c579c97349e544890626770ab1aa448d8d081d3cdd3735342060
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153059206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ef815aafcd5e327a9fc3d4d98037b2c4e5663014cc1fa58a9e2c11d040ff96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 20:34:29 GMT
ADD file:b269dd25aa5a2b39f29e341376ca9f2b8aded8f1327c01024b96a2eaa5c3a142 in / 
# Thu, 15 Feb 2018 20:34:29 GMT
CMD ["bash"]
# Fri, 16 Feb 2018 11:39:49 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Fri, 16 Feb 2018 11:39:50 GMT
ENV MONO_VERSION=4.8.0.524
# Fri, 16 Feb 2018 11:40:06 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Fri, 16 Feb 2018 11:40:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Fri, 16 Feb 2018 11:41:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f10fe2356c6af971fa6e4de75405f5f2c0a1b4dd473c5da5cca0dc476bf491f8`  
		Last Modified: Thu, 15 Feb 2018 01:29:03 GMT  
		Size: 37.4 MB (37439124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e617752d4f547c030861e5d17fe22d2a1a97a5719106a706bb9087aab6788984`  
		Last Modified: Fri, 16 Feb 2018 12:04:35 GMT  
		Size: 9.6 MB (9607507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0c5d1b4144aae8c52ba8fd6fbb632e1e4bb1ad1938e34fcf51b791efc2937b`  
		Last Modified: Fri, 16 Feb 2018 12:04:31 GMT  
		Size: 29.9 KB (29908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8323e44890fa0ebf489071f9912d8e2339baab4ba4395fd35a51b71c2d63825`  
		Last Modified: Fri, 16 Feb 2018 12:05:14 GMT  
		Size: 106.0 MB (105982667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5`

```console
$ docker pull mono@sha256:7eb698a27f6de28ffdc65b9e8b29282b10ee93bf3e0c1622c2d1fbada4af87ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5` - linux; amd64

```console
$ docker pull mono@sha256:86b874309abb9e292c361e12a68f5033f7bfa68c8ffc32a6b8950466926564b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174624749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90d81585b35567261136b5f2e96fe9b8da4e5468974c32ccba0207aa2e0ac6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:33:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead69961751b24ab2d3dd7c5de6cef3032cbb60805a2b74631e97c3cf20581fc`  
		Last Modified: Wed, 14 Mar 2018 07:41:46 GMT  
		Size: 117.1 MB (117137776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9c3bce310eaabae961419780138801c92ace40bbb58f576e337f147389d2fb03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168760444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb6eb80e935bf4b4486a8046d62c2ba170d2b9fc06fdf99f7a25f7740b70e49`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90485d367026a123593f0b38e0742b10df0a9f6179acffb54a994d6f72a76428`  
		Last Modified: Wed, 14 Mar 2018 22:20:13 GMT  
		Size: 115.0 MB (115011967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; 386

```console
$ docker pull mono@sha256:d7c9568f926aa763dbcc613d63827a9558e25cd3617f670fb3deb07442ce1ff7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176848161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35810e1d40a00dd235ed947b13e6457a629cea1439a5f0471775a4eb136c64e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 27 Feb 2018 02:09:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64310fe25d5665f939a1a8e651bad1b34ac87f1bc0fca6b6017e514697e3e2b1`  
		Last Modified: Tue, 27 Feb 2018 03:00:55 GMT  
		Size: 117.4 MB (117437070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4`

```console
$ docker pull mono@sha256:2fe187d8fe3bf4e0f922b8a0e493b8bc538ff50e8c5548a6d991bd0be90ee666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4` - linux; amd64

```console
$ docker pull mono@sha256:952466c6a038fe198d305a07010723e4b10fbac844195d29a8ab18d1b768b8e7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167265378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e1934aeebbec1b21dc32de92af947be1c1c2958cdb7c7422da49f5d04e071a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:23:39 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 07:23:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:24:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:36:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f924ca5279fae3fd3d71622a27021c791fa823dfe044d361dfb16626e29b`  
		Last Modified: Wed, 14 Mar 2018 07:38:37 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e614f17e8687dc6b4390e4924c68c0dc0e714a99ef7ebba1d358c0564a7c1d`  
		Last Modified: Wed, 14 Mar 2018 07:38:45 GMT  
		Size: 27.3 MB (27278932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9092becf199dd4902ddb90008d60724d4d92c1eb29a8ca0e8dcf1ea944f79`  
		Last Modified: Wed, 14 Mar 2018 07:43:39 GMT  
		Size: 109.9 MB (109861981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4` - linux; arm variant v7

```console
$ docker pull mono@sha256:8fab2a1518e04f12109196a89fa2591f117bc01ee5abcd4a8fd12fb3a109e66a
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147041676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdda3773dfe3f7aa7d781e845ebb2505b06993f035c3998af6b2f024e1c35b13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:47 GMT
ADD file:1f5de474caa19da14d698a3f9c3d161abfa1e19e258a596d64f3dfc9e2f17686 in / 
# Tue, 12 Dec 2017 13:27:47 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:39:27 GMT
ENV MONO_VERSION=5.4.1.6
# Tue, 12 Dec 2017 14:39:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 12 Dec 2017 14:40:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Dec 2017 14:46:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b9c0f1a415433a98643bdda391dcf4fe5d9653fc3ed3845c7ac1be99eb43399`  
		Last Modified: Tue, 12 Dec 2017 13:39:52 GMT  
		Size: 26.3 MB (26282714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23710a344ee6760b7342ca472bb26f9421156ff324fe5a96de2f0450c85c10f`  
		Last Modified: Tue, 12 Dec 2017 14:49:07 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea55960f594bf57ce8f8ba10b6b29e72cc44a6cdf3df27808c200f325c258bf1`  
		Last Modified: Tue, 12 Dec 2017 14:49:15 GMT  
		Size: 22.0 MB (22035209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b74f680ad16dc3a0219a3b0844435b615ede5416ae17ef48a099f54b1c72f4`  
		Last Modified: Tue, 12 Dec 2017 14:52:47 GMT  
		Size: 98.7 MB (98721690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a54260d7b384b2557b8f5f825885105094a9c0b0f546c228bd0c8f9d8c8933b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161647648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c86dc7fb3a0bb9328a19c5a39a63c4bd2ed76b1d6d947e9f163955fe8343be70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:56:18 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 21:56:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:58:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:15:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49decf9f81a8296b3afa7cdeb614e475aa9f1da662687e6ddeb600b02a8279a0`  
		Last Modified: Wed, 14 Mar 2018 22:18:20 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b450456ca88e087941838940f78d2c8ffa406d8da8f04c8190dca3c0b66921`  
		Last Modified: Wed, 14 Mar 2018 22:18:31 GMT  
		Size: 26.2 MB (26196770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff87fe00a08ac51bbc2659b0deb2a75e063dcb16845d529d3e9d44693d78348`  
		Last Modified: Wed, 14 Mar 2018 22:22:24 GMT  
		Size: 108.0 MB (107960635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4` - linux; 386

```console
$ docker pull mono@sha256:17bccf42a94f0c2feedabc40ab5f0098d23560c9948387eabbec8aea2f85f8d5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.7 MB (169654413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43233013d56a6267b22812e2c17b30735af303969ff65c39c56a5c3adc21e5d4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Wed, 21 Feb 2018 07:35:52 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 21 Feb 2018 07:36:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 21 Feb 2018 07:36:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 21 Feb 2018 07:58:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e13325bb17a7c5bf15f6cd5c2ea2edd25eaf513eb88681087bb8546954a84fa`  
		Last Modified: Wed, 21 Feb 2018 08:37:30 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b27874c1243e77489b4bc666802b53271f16e0a2a1d0ab3f2fda2f0cd2a077`  
		Last Modified: Wed, 21 Feb 2018 08:37:42 GMT  
		Size: 29.1 MB (29054103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6407ba77826c131ff0941af1faeb13aeb329e2f3e8ab7376c232d92e7244`  
		Last Modified: Wed, 21 Feb 2018 08:49:57 GMT  
		Size: 110.3 MB (110325043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.1`

```console
$ docker pull mono@sha256:2fe187d8fe3bf4e0f922b8a0e493b8bc538ff50e8c5548a6d991bd0be90ee666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.1` - linux; amd64

```console
$ docker pull mono@sha256:952466c6a038fe198d305a07010723e4b10fbac844195d29a8ab18d1b768b8e7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167265378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e1934aeebbec1b21dc32de92af947be1c1c2958cdb7c7422da49f5d04e071a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:23:39 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 07:23:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:24:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:36:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f924ca5279fae3fd3d71622a27021c791fa823dfe044d361dfb16626e29b`  
		Last Modified: Wed, 14 Mar 2018 07:38:37 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e614f17e8687dc6b4390e4924c68c0dc0e714a99ef7ebba1d358c0564a7c1d`  
		Last Modified: Wed, 14 Mar 2018 07:38:45 GMT  
		Size: 27.3 MB (27278932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9092becf199dd4902ddb90008d60724d4d92c1eb29a8ca0e8dcf1ea944f79`  
		Last Modified: Wed, 14 Mar 2018 07:43:39 GMT  
		Size: 109.9 MB (109861981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1` - linux; arm variant v7

```console
$ docker pull mono@sha256:8fab2a1518e04f12109196a89fa2591f117bc01ee5abcd4a8fd12fb3a109e66a
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147041676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdda3773dfe3f7aa7d781e845ebb2505b06993f035c3998af6b2f024e1c35b13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:47 GMT
ADD file:1f5de474caa19da14d698a3f9c3d161abfa1e19e258a596d64f3dfc9e2f17686 in / 
# Tue, 12 Dec 2017 13:27:47 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:39:27 GMT
ENV MONO_VERSION=5.4.1.6
# Tue, 12 Dec 2017 14:39:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 12 Dec 2017 14:40:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Dec 2017 14:46:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b9c0f1a415433a98643bdda391dcf4fe5d9653fc3ed3845c7ac1be99eb43399`  
		Last Modified: Tue, 12 Dec 2017 13:39:52 GMT  
		Size: 26.3 MB (26282714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23710a344ee6760b7342ca472bb26f9421156ff324fe5a96de2f0450c85c10f`  
		Last Modified: Tue, 12 Dec 2017 14:49:07 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea55960f594bf57ce8f8ba10b6b29e72cc44a6cdf3df27808c200f325c258bf1`  
		Last Modified: Tue, 12 Dec 2017 14:49:15 GMT  
		Size: 22.0 MB (22035209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b74f680ad16dc3a0219a3b0844435b615ede5416ae17ef48a099f54b1c72f4`  
		Last Modified: Tue, 12 Dec 2017 14:52:47 GMT  
		Size: 98.7 MB (98721690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a54260d7b384b2557b8f5f825885105094a9c0b0f546c228bd0c8f9d8c8933b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161647648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c86dc7fb3a0bb9328a19c5a39a63c4bd2ed76b1d6d947e9f163955fe8343be70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:56:18 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 21:56:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:58:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:15:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49decf9f81a8296b3afa7cdeb614e475aa9f1da662687e6ddeb600b02a8279a0`  
		Last Modified: Wed, 14 Mar 2018 22:18:20 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b450456ca88e087941838940f78d2c8ffa406d8da8f04c8190dca3c0b66921`  
		Last Modified: Wed, 14 Mar 2018 22:18:31 GMT  
		Size: 26.2 MB (26196770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff87fe00a08ac51bbc2659b0deb2a75e063dcb16845d529d3e9d44693d78348`  
		Last Modified: Wed, 14 Mar 2018 22:22:24 GMT  
		Size: 108.0 MB (107960635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1` - linux; 386

```console
$ docker pull mono@sha256:17bccf42a94f0c2feedabc40ab5f0098d23560c9948387eabbec8aea2f85f8d5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.7 MB (169654413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43233013d56a6267b22812e2c17b30735af303969ff65c39c56a5c3adc21e5d4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Wed, 21 Feb 2018 07:35:52 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 21 Feb 2018 07:36:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 21 Feb 2018 07:36:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 21 Feb 2018 07:58:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e13325bb17a7c5bf15f6cd5c2ea2edd25eaf513eb88681087bb8546954a84fa`  
		Last Modified: Wed, 21 Feb 2018 08:37:30 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b27874c1243e77489b4bc666802b53271f16e0a2a1d0ab3f2fda2f0cd2a077`  
		Last Modified: Wed, 21 Feb 2018 08:37:42 GMT  
		Size: 29.1 MB (29054103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6407ba77826c131ff0941af1faeb13aeb329e2f3e8ab7376c232d92e7244`  
		Last Modified: Wed, 21 Feb 2018 08:49:57 GMT  
		Size: 110.3 MB (110325043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.1.6`

```console
$ docker pull mono@sha256:2fe187d8fe3bf4e0f922b8a0e493b8bc538ff50e8c5548a6d991bd0be90ee666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.1.6` - linux; amd64

```console
$ docker pull mono@sha256:952466c6a038fe198d305a07010723e4b10fbac844195d29a8ab18d1b768b8e7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167265378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e1934aeebbec1b21dc32de92af947be1c1c2958cdb7c7422da49f5d04e071a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:23:39 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 07:23:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:24:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:36:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f924ca5279fae3fd3d71622a27021c791fa823dfe044d361dfb16626e29b`  
		Last Modified: Wed, 14 Mar 2018 07:38:37 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e614f17e8687dc6b4390e4924c68c0dc0e714a99ef7ebba1d358c0564a7c1d`  
		Last Modified: Wed, 14 Mar 2018 07:38:45 GMT  
		Size: 27.3 MB (27278932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9092becf199dd4902ddb90008d60724d4d92c1eb29a8ca0e8dcf1ea944f79`  
		Last Modified: Wed, 14 Mar 2018 07:43:39 GMT  
		Size: 109.9 MB (109861981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1.6` - linux; arm variant v7

```console
$ docker pull mono@sha256:8fab2a1518e04f12109196a89fa2591f117bc01ee5abcd4a8fd12fb3a109e66a
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147041676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdda3773dfe3f7aa7d781e845ebb2505b06993f035c3998af6b2f024e1c35b13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:47 GMT
ADD file:1f5de474caa19da14d698a3f9c3d161abfa1e19e258a596d64f3dfc9e2f17686 in / 
# Tue, 12 Dec 2017 13:27:47 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:39:27 GMT
ENV MONO_VERSION=5.4.1.6
# Tue, 12 Dec 2017 14:39:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 12 Dec 2017 14:40:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Dec 2017 14:46:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b9c0f1a415433a98643bdda391dcf4fe5d9653fc3ed3845c7ac1be99eb43399`  
		Last Modified: Tue, 12 Dec 2017 13:39:52 GMT  
		Size: 26.3 MB (26282714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23710a344ee6760b7342ca472bb26f9421156ff324fe5a96de2f0450c85c10f`  
		Last Modified: Tue, 12 Dec 2017 14:49:07 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea55960f594bf57ce8f8ba10b6b29e72cc44a6cdf3df27808c200f325c258bf1`  
		Last Modified: Tue, 12 Dec 2017 14:49:15 GMT  
		Size: 22.0 MB (22035209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b74f680ad16dc3a0219a3b0844435b615ede5416ae17ef48a099f54b1c72f4`  
		Last Modified: Tue, 12 Dec 2017 14:52:47 GMT  
		Size: 98.7 MB (98721690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1.6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a54260d7b384b2557b8f5f825885105094a9c0b0f546c228bd0c8f9d8c8933b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161647648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c86dc7fb3a0bb9328a19c5a39a63c4bd2ed76b1d6d947e9f163955fe8343be70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:56:18 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 21:56:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:58:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:15:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49decf9f81a8296b3afa7cdeb614e475aa9f1da662687e6ddeb600b02a8279a0`  
		Last Modified: Wed, 14 Mar 2018 22:18:20 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b450456ca88e087941838940f78d2c8ffa406d8da8f04c8190dca3c0b66921`  
		Last Modified: Wed, 14 Mar 2018 22:18:31 GMT  
		Size: 26.2 MB (26196770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff87fe00a08ac51bbc2659b0deb2a75e063dcb16845d529d3e9d44693d78348`  
		Last Modified: Wed, 14 Mar 2018 22:22:24 GMT  
		Size: 108.0 MB (107960635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1.6` - linux; 386

```console
$ docker pull mono@sha256:17bccf42a94f0c2feedabc40ab5f0098d23560c9948387eabbec8aea2f85f8d5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.7 MB (169654413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43233013d56a6267b22812e2c17b30735af303969ff65c39c56a5c3adc21e5d4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Wed, 21 Feb 2018 07:35:52 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 21 Feb 2018 07:36:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 21 Feb 2018 07:36:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 21 Feb 2018 07:58:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e13325bb17a7c5bf15f6cd5c2ea2edd25eaf513eb88681087bb8546954a84fa`  
		Last Modified: Wed, 21 Feb 2018 08:37:30 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b27874c1243e77489b4bc666802b53271f16e0a2a1d0ab3f2fda2f0cd2a077`  
		Last Modified: Wed, 21 Feb 2018 08:37:42 GMT  
		Size: 29.1 MB (29054103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6407ba77826c131ff0941af1faeb13aeb329e2f3e8ab7376c232d92e7244`  
		Last Modified: Wed, 21 Feb 2018 08:49:57 GMT  
		Size: 110.3 MB (110325043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.1.6-slim`

```console
$ docker pull mono@sha256:cc666edbbe54c7767594661f2233f3bd9079954ba3f7f643ff200c5201817aee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.1.6-slim` - linux; amd64

```console
$ docker pull mono@sha256:cadfae35c8dd651ff610f67c32e52a76134be85aaa4392e3c51a69fa7e9ffca1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57403397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e37862545268101f08eaebf7216716d3d258fc64326bc41ae2f402f1613adc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:23:39 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 07:23:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:24:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f924ca5279fae3fd3d71622a27021c791fa823dfe044d361dfb16626e29b`  
		Last Modified: Wed, 14 Mar 2018 07:38:37 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e614f17e8687dc6b4390e4924c68c0dc0e714a99ef7ebba1d358c0564a7c1d`  
		Last Modified: Wed, 14 Mar 2018 07:38:45 GMT  
		Size: 27.3 MB (27278932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1.6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:2e316966a653ca8041bddbd647ac350b2bc2c99e0c425df792b9b4414cebc1c8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48030002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b95acee6a82d0708f31715153678734944fde57b5c1358db79eba945f7fd78c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:27:25 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 13:27:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:28:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64568fb34d1015d379505d5efa6555265ef3eb8807aa8dacdc6a55a897cf4786`  
		Last Modified: Wed, 14 Mar 2018 13:45:13 GMT  
		Size: 2.1 KB (2070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78ce8cc2f889d0258394b0d8f199920b641538a9461278f564f73f981750f26`  
		Last Modified: Wed, 14 Mar 2018 13:45:22 GMT  
		Size: 21.7 MB (21737649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1.6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d29213717fafe69b351f05e828d2752771dd0275c85dcfc959296c4e3fc9fa2b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53687013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bce9557b48f4ed9653d1b8d0bcb0f47bf2799bc15a48cedeb32de43b470ffa9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:56:18 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 21:56:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:58:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49decf9f81a8296b3afa7cdeb614e475aa9f1da662687e6ddeb600b02a8279a0`  
		Last Modified: Wed, 14 Mar 2018 22:18:20 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b450456ca88e087941838940f78d2c8ffa406d8da8f04c8190dca3c0b66921`  
		Last Modified: Wed, 14 Mar 2018 22:18:31 GMT  
		Size: 26.2 MB (26196770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1.6-slim` - linux; 386

```console
$ docker pull mono@sha256:8e700528cb6fd353da4aa008977d6ef770597423b36dc7c0cc5ff153048c0200
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59329370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8876795c0a3f11b961d36090142150fd6ff7baa4960e761776686ed487d1e70b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Wed, 21 Feb 2018 07:35:52 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 21 Feb 2018 07:36:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 21 Feb 2018 07:36:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e13325bb17a7c5bf15f6cd5c2ea2edd25eaf513eb88681087bb8546954a84fa`  
		Last Modified: Wed, 21 Feb 2018 08:37:30 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b27874c1243e77489b4bc666802b53271f16e0a2a1d0ab3f2fda2f0cd2a077`  
		Last Modified: Wed, 21 Feb 2018 08:37:42 GMT  
		Size: 29.1 MB (29054103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.1-slim`

```console
$ docker pull mono@sha256:cc666edbbe54c7767594661f2233f3bd9079954ba3f7f643ff200c5201817aee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.1-slim` - linux; amd64

```console
$ docker pull mono@sha256:cadfae35c8dd651ff610f67c32e52a76134be85aaa4392e3c51a69fa7e9ffca1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57403397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e37862545268101f08eaebf7216716d3d258fc64326bc41ae2f402f1613adc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:23:39 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 07:23:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:24:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f924ca5279fae3fd3d71622a27021c791fa823dfe044d361dfb16626e29b`  
		Last Modified: Wed, 14 Mar 2018 07:38:37 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e614f17e8687dc6b4390e4924c68c0dc0e714a99ef7ebba1d358c0564a7c1d`  
		Last Modified: Wed, 14 Mar 2018 07:38:45 GMT  
		Size: 27.3 MB (27278932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:2e316966a653ca8041bddbd647ac350b2bc2c99e0c425df792b9b4414cebc1c8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48030002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b95acee6a82d0708f31715153678734944fde57b5c1358db79eba945f7fd78c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:27:25 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 13:27:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:28:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64568fb34d1015d379505d5efa6555265ef3eb8807aa8dacdc6a55a897cf4786`  
		Last Modified: Wed, 14 Mar 2018 13:45:13 GMT  
		Size: 2.1 KB (2070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78ce8cc2f889d0258394b0d8f199920b641538a9461278f564f73f981750f26`  
		Last Modified: Wed, 14 Mar 2018 13:45:22 GMT  
		Size: 21.7 MB (21737649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d29213717fafe69b351f05e828d2752771dd0275c85dcfc959296c4e3fc9fa2b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53687013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bce9557b48f4ed9653d1b8d0bcb0f47bf2799bc15a48cedeb32de43b470ffa9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:56:18 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 21:56:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:58:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49decf9f81a8296b3afa7cdeb614e475aa9f1da662687e6ddeb600b02a8279a0`  
		Last Modified: Wed, 14 Mar 2018 22:18:20 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b450456ca88e087941838940f78d2c8ffa406d8da8f04c8190dca3c0b66921`  
		Last Modified: Wed, 14 Mar 2018 22:18:31 GMT  
		Size: 26.2 MB (26196770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.1-slim` - linux; 386

```console
$ docker pull mono@sha256:8e700528cb6fd353da4aa008977d6ef770597423b36dc7c0cc5ff153048c0200
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59329370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8876795c0a3f11b961d36090142150fd6ff7baa4960e761776686ed487d1e70b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Wed, 21 Feb 2018 07:35:52 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 21 Feb 2018 07:36:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 21 Feb 2018 07:36:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e13325bb17a7c5bf15f6cd5c2ea2edd25eaf513eb88681087bb8546954a84fa`  
		Last Modified: Wed, 21 Feb 2018 08:37:30 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b27874c1243e77489b4bc666802b53271f16e0a2a1d0ab3f2fda2f0cd2a077`  
		Last Modified: Wed, 21 Feb 2018 08:37:42 GMT  
		Size: 29.1 MB (29054103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4-slim`

```console
$ docker pull mono@sha256:cc666edbbe54c7767594661f2233f3bd9079954ba3f7f643ff200c5201817aee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4-slim` - linux; amd64

```console
$ docker pull mono@sha256:cadfae35c8dd651ff610f67c32e52a76134be85aaa4392e3c51a69fa7e9ffca1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57403397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e37862545268101f08eaebf7216716d3d258fc64326bc41ae2f402f1613adc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:23:39 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 07:23:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:24:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f924ca5279fae3fd3d71622a27021c791fa823dfe044d361dfb16626e29b`  
		Last Modified: Wed, 14 Mar 2018 07:38:37 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e614f17e8687dc6b4390e4924c68c0dc0e714a99ef7ebba1d358c0564a7c1d`  
		Last Modified: Wed, 14 Mar 2018 07:38:45 GMT  
		Size: 27.3 MB (27278932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:2e316966a653ca8041bddbd647ac350b2bc2c99e0c425df792b9b4414cebc1c8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48030002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b95acee6a82d0708f31715153678734944fde57b5c1358db79eba945f7fd78c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:27:25 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 13:27:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:28:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64568fb34d1015d379505d5efa6555265ef3eb8807aa8dacdc6a55a897cf4786`  
		Last Modified: Wed, 14 Mar 2018 13:45:13 GMT  
		Size: 2.1 KB (2070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78ce8cc2f889d0258394b0d8f199920b641538a9461278f564f73f981750f26`  
		Last Modified: Wed, 14 Mar 2018 13:45:22 GMT  
		Size: 21.7 MB (21737649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d29213717fafe69b351f05e828d2752771dd0275c85dcfc959296c4e3fc9fa2b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53687013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bce9557b48f4ed9653d1b8d0bcb0f47bf2799bc15a48cedeb32de43b470ffa9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:56:18 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 14 Mar 2018 21:56:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:58:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49decf9f81a8296b3afa7cdeb614e475aa9f1da662687e6ddeb600b02a8279a0`  
		Last Modified: Wed, 14 Mar 2018 22:18:20 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b450456ca88e087941838940f78d2c8ffa406d8da8f04c8190dca3c0b66921`  
		Last Modified: Wed, 14 Mar 2018 22:18:31 GMT  
		Size: 26.2 MB (26196770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4-slim` - linux; 386

```console
$ docker pull mono@sha256:8e700528cb6fd353da4aa008977d6ef770597423b36dc7c0cc5ff153048c0200
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59329370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8876795c0a3f11b961d36090142150fd6ff7baa4960e761776686ed487d1e70b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Wed, 21 Feb 2018 07:35:52 GMT
ENV MONO_VERSION=5.4.1.6
# Wed, 21 Feb 2018 07:36:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 21 Feb 2018 07:36:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e13325bb17a7c5bf15f6cd5c2ea2edd25eaf513eb88681087bb8546954a84fa`  
		Last Modified: Wed, 21 Feb 2018 08:37:30 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b27874c1243e77489b4bc666802b53271f16e0a2a1d0ab3f2fda2f0cd2a077`  
		Last Modified: Wed, 21 Feb 2018 08:37:42 GMT  
		Size: 29.1 MB (29054103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.8`

```console
$ docker pull mono@sha256:7eb698a27f6de28ffdc65b9e8b29282b10ee93bf3e0c1622c2d1fbada4af87ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.8` - linux; amd64

```console
$ docker pull mono@sha256:86b874309abb9e292c361e12a68f5033f7bfa68c8ffc32a6b8950466926564b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174624749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90d81585b35567261136b5f2e96fe9b8da4e5468974c32ccba0207aa2e0ac6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:33:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead69961751b24ab2d3dd7c5de6cef3032cbb60805a2b74631e97c3cf20581fc`  
		Last Modified: Wed, 14 Mar 2018 07:41:46 GMT  
		Size: 117.1 MB (117137776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9c3bce310eaabae961419780138801c92ace40bbb58f576e337f147389d2fb03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168760444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb6eb80e935bf4b4486a8046d62c2ba170d2b9fc06fdf99f7a25f7740b70e49`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90485d367026a123593f0b38e0742b10df0a9f6179acffb54a994d6f72a76428`  
		Last Modified: Wed, 14 Mar 2018 22:20:13 GMT  
		Size: 115.0 MB (115011967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8` - linux; 386

```console
$ docker pull mono@sha256:d7c9568f926aa763dbcc613d63827a9558e25cd3617f670fb3deb07442ce1ff7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176848161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35810e1d40a00dd235ed947b13e6457a629cea1439a5f0471775a4eb136c64e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 27 Feb 2018 02:09:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64310fe25d5665f939a1a8e651bad1b34ac87f1bc0fca6b6017e514697e3e2b1`  
		Last Modified: Tue, 27 Feb 2018 03:00:55 GMT  
		Size: 117.4 MB (117437070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.8.0`

```console
$ docker pull mono@sha256:7eb698a27f6de28ffdc65b9e8b29282b10ee93bf3e0c1622c2d1fbada4af87ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.8.0` - linux; amd64

```console
$ docker pull mono@sha256:86b874309abb9e292c361e12a68f5033f7bfa68c8ffc32a6b8950466926564b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174624749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90d81585b35567261136b5f2e96fe9b8da4e5468974c32ccba0207aa2e0ac6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:33:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead69961751b24ab2d3dd7c5de6cef3032cbb60805a2b74631e97c3cf20581fc`  
		Last Modified: Wed, 14 Mar 2018 07:41:46 GMT  
		Size: 117.1 MB (117137776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9c3bce310eaabae961419780138801c92ace40bbb58f576e337f147389d2fb03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168760444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb6eb80e935bf4b4486a8046d62c2ba170d2b9fc06fdf99f7a25f7740b70e49`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90485d367026a123593f0b38e0742b10df0a9f6179acffb54a994d6f72a76428`  
		Last Modified: Wed, 14 Mar 2018 22:20:13 GMT  
		Size: 115.0 MB (115011967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0` - linux; 386

```console
$ docker pull mono@sha256:d7c9568f926aa763dbcc613d63827a9558e25cd3617f670fb3deb07442ce1ff7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176848161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35810e1d40a00dd235ed947b13e6457a629cea1439a5f0471775a4eb136c64e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 27 Feb 2018 02:09:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64310fe25d5665f939a1a8e651bad1b34ac87f1bc0fca6b6017e514697e3e2b1`  
		Last Modified: Tue, 27 Feb 2018 03:00:55 GMT  
		Size: 117.4 MB (117437070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.8.0.127`

```console
$ docker pull mono@sha256:7eb698a27f6de28ffdc65b9e8b29282b10ee93bf3e0c1622c2d1fbada4af87ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.8.0.127` - linux; amd64

```console
$ docker pull mono@sha256:86b874309abb9e292c361e12a68f5033f7bfa68c8ffc32a6b8950466926564b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174624749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90d81585b35567261136b5f2e96fe9b8da4e5468974c32ccba0207aa2e0ac6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:33:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead69961751b24ab2d3dd7c5de6cef3032cbb60805a2b74631e97c3cf20581fc`  
		Last Modified: Wed, 14 Mar 2018 07:41:46 GMT  
		Size: 117.1 MB (117137776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0.127` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9c3bce310eaabae961419780138801c92ace40bbb58f576e337f147389d2fb03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168760444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb6eb80e935bf4b4486a8046d62c2ba170d2b9fc06fdf99f7a25f7740b70e49`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90485d367026a123593f0b38e0742b10df0a9f6179acffb54a994d6f72a76428`  
		Last Modified: Wed, 14 Mar 2018 22:20:13 GMT  
		Size: 115.0 MB (115011967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0.127` - linux; 386

```console
$ docker pull mono@sha256:d7c9568f926aa763dbcc613d63827a9558e25cd3617f670fb3deb07442ce1ff7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176848161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35810e1d40a00dd235ed947b13e6457a629cea1439a5f0471775a4eb136c64e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 27 Feb 2018 02:09:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64310fe25d5665f939a1a8e651bad1b34ac87f1bc0fca6b6017e514697e3e2b1`  
		Last Modified: Tue, 27 Feb 2018 03:00:55 GMT  
		Size: 117.4 MB (117437070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.8.0.127-slim`

```console
$ docker pull mono@sha256:92f06730cc999a2d566315a4557da34b6bb111a01a5626017be9e47f906bcd77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.8.0.127-slim` - linux; amd64

```console
$ docker pull mono@sha256:05d8988c6bb3d226ebb47288f62940c86f57381c81742323e3f08b80f4e8f970
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57486973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a675dd8c202444a1867e7c27a1cfbd54c36dad5d58f1666d82bb1a27692857c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0.127-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:cbce71ca8ff422141b6bf217538b1be55110371a37f28db113e2ea25605d0e10
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48075464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf37d0030b80af9febd20a44a4d503b7c413611343ff06dc8919d1468a36046`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:25:50 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 13:25:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:26:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506744380672d33996ae5adb48ca8f8a6da341f44d2269cdf707fb1a168692e`  
		Last Modified: Wed, 14 Mar 2018 13:44:02 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c841cb48c5e18d2b76f8548d756020648a121a1e67d1e12eab1ef0a59d6b80`  
		Last Modified: Wed, 14 Mar 2018 13:44:10 GMT  
		Size: 21.8 MB (21783117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0.127-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:81bd13fad36e5faa9441fd4372ce2d0da7c9f72c0627160ba76a02db2a2e64f3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53748477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88c82e847e5225e60cda929e8f0c094cc1ba1451d62201b554aa365437943765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0.127-slim` - linux; 386

```console
$ docker pull mono@sha256:8bb8ce19f4582610e3ec948d11bb21bac165fed4579f4ee788cccc58426c6860
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59411091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09319bcc376925b78d888cf200bc523a691db4a7e289349dba5d32a3e723fbed`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.8.0-slim`

```console
$ docker pull mono@sha256:92f06730cc999a2d566315a4557da34b6bb111a01a5626017be9e47f906bcd77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.8.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:05d8988c6bb3d226ebb47288f62940c86f57381c81742323e3f08b80f4e8f970
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57486973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a675dd8c202444a1867e7c27a1cfbd54c36dad5d58f1666d82bb1a27692857c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:cbce71ca8ff422141b6bf217538b1be55110371a37f28db113e2ea25605d0e10
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48075464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf37d0030b80af9febd20a44a4d503b7c413611343ff06dc8919d1468a36046`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:25:50 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 13:25:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:26:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506744380672d33996ae5adb48ca8f8a6da341f44d2269cdf707fb1a168692e`  
		Last Modified: Wed, 14 Mar 2018 13:44:02 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c841cb48c5e18d2b76f8548d756020648a121a1e67d1e12eab1ef0a59d6b80`  
		Last Modified: Wed, 14 Mar 2018 13:44:10 GMT  
		Size: 21.8 MB (21783117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:81bd13fad36e5faa9441fd4372ce2d0da7c9f72c0627160ba76a02db2a2e64f3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53748477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88c82e847e5225e60cda929e8f0c094cc1ba1451d62201b554aa365437943765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8.0-slim` - linux; 386

```console
$ docker pull mono@sha256:8bb8ce19f4582610e3ec948d11bb21bac165fed4579f4ee788cccc58426c6860
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59411091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09319bcc376925b78d888cf200bc523a691db4a7e289349dba5d32a3e723fbed`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.8-slim`

```console
$ docker pull mono@sha256:92f06730cc999a2d566315a4557da34b6bb111a01a5626017be9e47f906bcd77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.8-slim` - linux; amd64

```console
$ docker pull mono@sha256:05d8988c6bb3d226ebb47288f62940c86f57381c81742323e3f08b80f4e8f970
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57486973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a675dd8c202444a1867e7c27a1cfbd54c36dad5d58f1666d82bb1a27692857c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:cbce71ca8ff422141b6bf217538b1be55110371a37f28db113e2ea25605d0e10
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48075464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf37d0030b80af9febd20a44a4d503b7c413611343ff06dc8919d1468a36046`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:25:50 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 13:25:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:26:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506744380672d33996ae5adb48ca8f8a6da341f44d2269cdf707fb1a168692e`  
		Last Modified: Wed, 14 Mar 2018 13:44:02 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c841cb48c5e18d2b76f8548d756020648a121a1e67d1e12eab1ef0a59d6b80`  
		Last Modified: Wed, 14 Mar 2018 13:44:10 GMT  
		Size: 21.8 MB (21783117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:81bd13fad36e5faa9441fd4372ce2d0da7c9f72c0627160ba76a02db2a2e64f3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53748477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88c82e847e5225e60cda929e8f0c094cc1ba1451d62201b554aa365437943765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.8-slim` - linux; 386

```console
$ docker pull mono@sha256:8bb8ce19f4582610e3ec948d11bb21bac165fed4579f4ee788cccc58426c6860
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59411091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09319bcc376925b78d888cf200bc523a691db4a7e289349dba5d32a3e723fbed`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5-slim`

```console
$ docker pull mono@sha256:92f06730cc999a2d566315a4557da34b6bb111a01a5626017be9e47f906bcd77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5-slim` - linux; amd64

```console
$ docker pull mono@sha256:05d8988c6bb3d226ebb47288f62940c86f57381c81742323e3f08b80f4e8f970
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57486973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a675dd8c202444a1867e7c27a1cfbd54c36dad5d58f1666d82bb1a27692857c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:cbce71ca8ff422141b6bf217538b1be55110371a37f28db113e2ea25605d0e10
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48075464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf37d0030b80af9febd20a44a4d503b7c413611343ff06dc8919d1468a36046`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:25:50 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 13:25:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:26:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506744380672d33996ae5adb48ca8f8a6da341f44d2269cdf707fb1a168692e`  
		Last Modified: Wed, 14 Mar 2018 13:44:02 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c841cb48c5e18d2b76f8548d756020648a121a1e67d1e12eab1ef0a59d6b80`  
		Last Modified: Wed, 14 Mar 2018 13:44:10 GMT  
		Size: 21.8 MB (21783117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:81bd13fad36e5faa9441fd4372ce2d0da7c9f72c0627160ba76a02db2a2e64f3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53748477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88c82e847e5225e60cda929e8f0c094cc1ba1451d62201b554aa365437943765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; 386

```console
$ docker pull mono@sha256:8bb8ce19f4582610e3ec948d11bb21bac165fed4579f4ee788cccc58426c6860
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59411091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09319bcc376925b78d888cf200bc523a691db4a7e289349dba5d32a3e723fbed`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:7eb698a27f6de28ffdc65b9e8b29282b10ee93bf3e0c1622c2d1fbada4af87ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:latest` - linux; amd64

```console
$ docker pull mono@sha256:86b874309abb9e292c361e12a68f5033f7bfa68c8ffc32a6b8950466926564b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174624749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90d81585b35567261136b5f2e96fe9b8da4e5468974c32ccba0207aa2e0ac6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 07:33:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead69961751b24ab2d3dd7c5de6cef3032cbb60805a2b74631e97c3cf20581fc`  
		Last Modified: Wed, 14 Mar 2018 07:41:46 GMT  
		Size: 117.1 MB (117137776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9c3bce310eaabae961419780138801c92ace40bbb58f576e337f147389d2fb03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168760444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb6eb80e935bf4b4486a8046d62c2ba170d2b9fc06fdf99f7a25f7740b70e49`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 14 Mar 2018 22:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90485d367026a123593f0b38e0742b10df0a9f6179acffb54a994d6f72a76428`  
		Last Modified: Wed, 14 Mar 2018 22:20:13 GMT  
		Size: 115.0 MB (115011967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:d7c9568f926aa763dbcc613d63827a9558e25cd3617f670fb3deb07442ce1ff7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176848161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35810e1d40a00dd235ed947b13e6457a629cea1439a5f0471775a4eb136c64e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 27 Feb 2018 02:09:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64310fe25d5665f939a1a8e651bad1b34ac87f1bc0fca6b6017e514697e3e2b1`  
		Last Modified: Tue, 27 Feb 2018 03:00:55 GMT  
		Size: 117.4 MB (117437070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:92f06730cc999a2d566315a4557da34b6bb111a01a5626017be9e47f906bcd77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:slim` - linux; amd64

```console
$ docker pull mono@sha256:05d8988c6bb3d226ebb47288f62940c86f57381c81742323e3f08b80f4e8f970
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57486973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a675dd8c202444a1867e7c27a1cfbd54c36dad5d58f1666d82bb1a27692857c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Mar 2018 21:58:13 GMT
ADD file:080bac9a2cdcc70ad61e50045a26172f0e1acfd3a26360cb86b6e26a3307b2e1 in / 
# Tue, 13 Mar 2018 21:58:13 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 07:21:47 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 07:21:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 07:23:13 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b0568b191983bc2844b2fdb48aeefa72452931bfead0a87e0515bfc602ea3b0c`  
		Last Modified: Tue, 13 Mar 2018 22:45:19 GMT  
		Size: 30.1 MB (30122402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fd5726edd9f3f1977b65a4821afb616d239e3319df8be009446488f7d4ce3`  
		Last Modified: Wed, 14 Mar 2018 07:37:01 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be731cda004b97c2050c943945d71afc8ad94d592dc429aaa3924191d1a632`  
		Last Modified: Wed, 14 Mar 2018 07:37:11 GMT  
		Size: 27.4 MB (27362503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:cbce71ca8ff422141b6bf217538b1be55110371a37f28db113e2ea25605d0e10
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48075464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf37d0030b80af9febd20a44a4d503b7c413611343ff06dc8919d1468a36046`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 12:27:28 GMT
ADD file:901c5a711f269a7dd8f11eff27131cd2f6d2aee98d68f1e19b4ed954798e5d3f in / 
# Wed, 14 Mar 2018 12:27:29 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 13:25:50 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 13:25:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 13:26:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b8c016a755ce56e2fbb5a9f179c7bde3f0742c21b2727356a1658fc7d973f46a`  
		Last Modified: Wed, 14 Mar 2018 12:39:21 GMT  
		Size: 26.3 MB (26290283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506744380672d33996ae5adb48ca8f8a6da341f44d2269cdf707fb1a168692e`  
		Last Modified: Wed, 14 Mar 2018 13:44:02 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c841cb48c5e18d2b76f8548d756020648a121a1e67d1e12eab1ef0a59d6b80`  
		Last Modified: Wed, 14 Mar 2018 13:44:10 GMT  
		Size: 21.8 MB (21783117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:81bd13fad36e5faa9441fd4372ce2d0da7c9f72c0627160ba76a02db2a2e64f3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53748477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88c82e847e5225e60cda929e8f0c094cc1ba1451d62201b554aa365437943765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Mar 2018 17:25:26 GMT
ADD file:0012468f66c7e5b0efd7217a1f29f5044d4dce5a19dcd39786aa7573bc927763 in / 
# Wed, 14 Mar 2018 17:25:26 GMT
CMD ["bash"]
# Wed, 14 Mar 2018 21:53:54 GMT
ENV MONO_VERSION=5.8.0.127
# Wed, 14 Mar 2018 21:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Wed, 14 Mar 2018 21:55:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:784b6f32f75d9222c618727f66027b44ffa35120fc128790dfce4d1070befc90`  
		Last Modified: Wed, 14 Mar 2018 17:39:37 GMT  
		Size: 27.5 MB (27488177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6b1367b2d1c9afa214a230ea52e7bae7b50e6c2f4284b3fd7015beb8f1754`  
		Last Modified: Wed, 14 Mar 2018 22:16:29 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baa15e7a3fae65ce6bf6d31d2d1a973d2545cf410b81d9d9340c4f3062abc9`  
		Last Modified: Wed, 14 Mar 2018 22:16:40 GMT  
		Size: 26.3 MB (26258233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:8bb8ce19f4582610e3ec948d11bb21bac165fed4579f4ee788cccc58426c6860
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59411091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09319bcc376925b78d888cf200bc523a691db4a7e289349dba5d32a3e723fbed`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 15 Feb 2018 15:10:21 GMT
ADD file:d01127592c252b8d04a3bc643ddd1053a3e9cd036c81aa31b53bf3f51b542f6a in / 
# Thu, 15 Feb 2018 15:10:21 GMT
CMD ["bash"]
# Tue, 27 Feb 2018 02:02:15 GMT
ENV MONO_VERSION=5.8.0.127
# Tue, 27 Feb 2018 02:02:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 27 Feb 2018 02:03:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2c3a67c6c38b2cc7ef92c7d27dfe86398e5a7297b5b0e03d825a82312b60bf9a`  
		Last Modified: Thu, 15 Feb 2018 00:53:43 GMT  
		Size: 30.3 MB (30273198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72821c254faa67c4e9c36b9aa8d9c34d88984036cd0d4cd776a83af2c3e1f93`  
		Last Modified: Tue, 27 Feb 2018 02:29:31 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63759fd1c514ea99227042c8db724ab962baa81d5b4a97c4f3eb45ad7875857`  
		Last Modified: Tue, 27 Feb 2018 02:29:42 GMT  
		Size: 29.1 MB (29135824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
