# asdf-php-aur

[PHP](https://www.php.net) plugin for [asdf](https://github.com/asdf-vm/asdf) for [AUR](https://aur.archlinux.org/) users.
It uses [paru](https://github.com/Morganamilo/paru) to install php versions form AUR repository, and allows you to use them with `asdf`.

## Requirements

 - [paru](https://github.com/Morganamilo/paru)

## Installation

```bash
asdf plugin-add php https://github.com/pbogut/asdf-php-aur.git
```

## Usage

Check [asdf](https://github.com/asdf-vm/asdf) readme for instructions on how to
install & manage versions.

## How it works

It installs selected php version from `AUR` using `paru`, and then creates symlinks for `asdf` to use. 

## Why?

[asdf-php](https://github.com/asdf-community/asdf-php) is nice but unfortunately some PHP versions not always compile and I don't think there is easy version to install extensions (I may be wrong). But the most annoying thing is that after few system updates eventually some lib is no longer compatible and php stops working and I can't easily update it.

I already have `AUR` packages for different PHP versions, so why don't use them? They are made for my system and I can keep them up to date with simple `paru -Syu`. They are updated with my system so they rarely get broken.

## License

MIT License;
The software is provided "as is", without warranty of any kind.
