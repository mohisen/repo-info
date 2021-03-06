## `python:2-windowsservercore-1709`

```console
$ docker pull python@sha256:f845aa123d9e80050bbc1bae75581120fc009795f1b70a6dc389e28ab50c1697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.309; amd64

### `python:2-windowsservercore-1709` - windows version 10.0.16299.309; amd64

```console
$ docker pull python@sha256:61f4b97c72f206e9177d615286369db5fdd18006c585f5ff4d94016d84847030
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3072814611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276fdfc60dbc13448ba2b8c587c69fb9f1e53c3f93acdeb2fdd811a4d1aa6e03`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Mon, 05 Mar 2018 03:12:43 GMT
RUN Install update 10.0.16299.309
# Wed, 14 Mar 2018 02:30:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Mar 2018 16:49:36 GMT
ENV PYTHON_VERSION=2.7.14
# Wed, 14 Mar 2018 16:49:37 GMT
ENV PYTHON_RELEASE=2.7.14
# Wed, 14 Mar 2018 16:51:32 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}.amd64.msi' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'python.msi'; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'python.msi', 			'/quiet', 			'/qn', 			'TARGETDIR=C:\Python', 			'ALLUSERS=1', 			'ADDLOCAL=DefaultFeature,Extensions,TclTk,Tools,PrependPath' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Mar 2018 16:51:33 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 14 Mar 2018 16:52:56 GMT
RUN Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri 'https://bootstrap.pypa.io/get-pip.py' -OutFile 'get-pip.py'; 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.';
# Wed, 14 Mar 2018 16:53:53 GMT
RUN pip install --no-cache-dir virtualenv
# Wed, 14 Mar 2018 16:53:54 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:85f53e48ded4065a2dbea91a8444ffe14a44776674c9e437439702f9982f045f`  
		Last Modified: Tue, 13 Mar 2018 01:07:51 GMT  
		Size: 745.0 MB (745003512 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1752d0f4f0a05997b1c402225ed814b05d5b6704edffd353a828a56dc79c64e5`  
		Last Modified: Wed, 14 Mar 2018 16:55:14 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4372e03debd45d90eced2fc2ba908a4cd774080221fbb0649b0e902f9ba58d2b`  
		Last Modified: Wed, 14 Mar 2018 16:58:10 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e2873b136bbf574756a436b18b1b0ea7f0ec29fa0020c46af499ff95d42d3`  
		Last Modified: Wed, 14 Mar 2018 16:58:09 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dcad7bc68379603e5a2cba860cdd1b7f7ccbef72d836df911bd5feb0090746`  
		Last Modified: Wed, 14 Mar 2018 16:58:27 GMT  
		Size: 38.2 MB (38174728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ddc7fe4d497f87850897299ff24c64b49f099d5bcf0e4f0bbc25a80758ceae`  
		Last Modified: Wed, 14 Mar 2018 16:58:06 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db07d40ec5933688bdb69a847e8b948ef1acd147d5da365c96efd35c806af9c2`  
		Last Modified: Wed, 14 Mar 2018 16:58:14 GMT  
		Size: 8.8 MB (8797321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e67bd8e7bcba0c9f602d6636b5f04abcd0d5e79c1daca400a9d5fb47cde7087`  
		Last Modified: Wed, 14 Mar 2018 16:58:08 GMT  
		Size: 6.5 MB (6532499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4fa51338983343d59fdb7c489d422f0485bd29c6a4ec9566d16b2472c3e0fb`  
		Last Modified: Wed, 14 Mar 2018 16:58:06 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
