# Dokku copy plugin

Copy a folder using the dokku command


## Install

```
dokku plugin:install https://github.com/ochorocho/dokku-storage-copy.git storage-copy
```

Add `%dokku ALL=(ALL) NOPASSWD:/bin/rm -rf /var/lib/dokku/data/storage/*` to a new sudoers file in /etc/sudoers.d/

## Usage

```
ssh -t dokku@example.com -- storage:copy /var/lib/dokku/data/storage/<volume folder> /var/lib/dokku/data/storage/<target folder>
```
