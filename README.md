## Original Respoitory: https://github.com/picodotdev/alis.git

This repo was cloned bare and then mirrored for personal use.

The master branch of this repo contains the original code from when it was mirrored.

### Minimum Script Usage

```
# Start the machine with the latest arch installation media
# loadkeys [keymap] 	# us
# curl -sL https://raw.githubusercontent.com/sjcahill/arch_linux_install/personal/download.sh | bash
# vim alis.conf
# ./alis.sh
```

### Advanced Script Usage

```
# Start the machine with the latest arch installation media
# loadkeys [us]
# iwctl --passphrase <password> station <wifi-interface-name> connect <wifi-essid>
# curl -sL https://raw.githubusercontent.com/sjcahill/arch_linux_install/personal/download.sh | bash
# vim alis.conf
# vim alis-packages.conf
# (It is probably best to install packages after the initial install and reboot)
# ./alis.sh
# .alish.reboot.sh
```

### Mirrored a bare clone of the original repository in order to customize for personal use

```
git clone --bare git@github.com:picodotdev/alis.git
cd alis.git
git push --mirror git@github.com:sjcahill/arch_linux_install.git
cd ..
rm -rf alis.git
```

### If you want pull updates from the original upstream repo later

```
cd arch_linux_install.git
git remote add public git@github.com:picodotdev/alis.git
git pull public master # Creates a merge commit
git push origin master
```

### There is also a way to create pull request at a later date

Need to look that one up.

