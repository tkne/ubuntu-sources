Ubuntu sources.list dotfiles
======

Working Ubuntu 14.04 (Trusty Tahr) - Ubuntu 22.04 (Jammy Jellyfish) sources.list dotfiles to replace the sources.list in your /etc/apt folder on your Ubuntu server.

> [!TIP]
> These sources use Ubuntu Japan Team URL links (jp.archive.ubuntu.com). If you are handling servers in the US (or elsewhere for that matter), please update you sources.list dotfile manually by exchanging the `jp.` portion of the URL to `us.` if you are in the US for example.

## Usage:
Navigate to the `/etc/apt` folder.
```bash
cd /etc/apt
```

</br>

Backup your current `sources.list` file first.
```bash
mv sources.list sources.list_old
```

</br>

**For Ubuntu 14.04 (Trusty Tahr)**
```bash
wget https://raw.githubusercontent.com/tkne/ubuntu-sources/main/sources.list.ubuntu1404 -O /etc/apt/sources.list
```

</br>

**For Ubuntu 16.04 (Xenial Xerus)**
```bash
wget https://raw.githubusercontent.com/tkne/ubuntu-sources/main/sources.list.ubuntu1604 -O /etc/apt/sources.list
```

</br>

**For Ubuntu 18.04 (Bionic Beaver)**
```bash
wget https://raw.githubusercontent.com/tkne/ubuntu-sources/main/sources.list.ubuntu1804 -O /etc/apt/sources.list
```

</br>

**For Ubuntu 20.04 (Focal Fossa)**
```bash
wget https://raw.githubusercontent.com/tkne/ubuntu-sources/main/sources.list.ubuntu2004 -O /etc/apt/sources.list
```

</br>

**For Ubuntu 22.04 (Jammy Jellyfish)**
```bash
wget https://raw.githubusercontent.com/tkne/ubuntu-sources/main/sources.list.ubuntu2204 -O /etc/apt/sources.list
```

</br>

Update from the new list:
```bash
apt update
```

</br>

Upgrade from the new list:
```bash
apt upgrade
```

</br>

You can also edit and/or update your existing `sources.list` file manually if you prefer to do it that way.