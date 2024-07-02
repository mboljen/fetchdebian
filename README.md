# fetchdebian

Download Debian installation media files


## Synopsis

The following command will download the corresponding Debian installer image file to the current working directory.

```console
$ fetchdebian [OPTION]... CODENAME...
```

Use one of the following codenames or a version number.

- `lenny`
- `squeeze`
- `jessie`
- `stretch`
- `buster`
- `bullseye`
- `bookworm`
- `trixie`

According to the current development status of Debian, you can use the following alternatives:

- `stable` for Debian 12 (codename `bookworm`)
- `testing` for Debian 13 (codename `trixie`)
- `oldstable` for Debian 11 (codename `bullseye`)
- `oldoldstable` for Debian 10 (codename `buster`)

Append the suffix `-live` is appended to the codename, the script will download the image file of the corresponding Debian Live system.


## Description

This script downloads the latest Debian installer image to the current working directory.


## Options

+ `-p` _path_

  Specify download directory.  Default is current working directory.

+ `-a` _arch_

  Select one of the following software architectures.  Default is `amd64`.

  - `amd64`
  - `arm64`
  - `armel`
  - `armhf`
  - `i386`
  - `mips`
  - `mips64el`
  - `mipsel`
  - `multi-arch`
  - `ppc64el`
  - `s390x`
  - `source`
  - `trace`

+ `-d` _desktop_

  Select one of the following desktop environments for Live systems.  Default is `gnome`.

  - `cinnamon`
  - `gnome`
  - `kde`
  - `lxde`
  - `lxqt`
  - `mate`
  - `standard`
  - `xfce`

+ `-u` _url_

  Specify the base URL of the download location.  Default is `https://cdimage.debian.org/cdimage`.

+ `-l` _rate_

  Specify the maximal download bandwidth.  The default is `4M`.

+ `-h`

  Shows this help message.


## Installation

Use the following command to install this software:

```console
$ make
$ make install
```

The default `PREFIX` is set to `/usr/local`.  In order to successfully complete the installation, you need to have write permissions for the installation location.


## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.


## License

[MIT](https://choosealicense.com/licenses/mit/)
