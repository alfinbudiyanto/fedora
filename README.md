# Fedora
#### I prefer to install LibreOffice from flatpak
```
flatpak install falthub com.libreoffice.LibreOffice
```
so the group installed only 4

```
╭─ wolfei@fedora ~
╰─❯ fglh --installed

Updating and loading repositories:
Repositories loaded.
ID                        Name                             Installed
core                      Core                                   yes
hardware-support          Hardware Support                       yes
multimedia                Multimedia                             yes
networkmanager-submodules Common NetworkManager Submodules       yes
printing                  Printing Support                       yes
```
#### why only 4?,,
core is not count because it is fedora based

### For aliases was i made
```
alias fgl = "dnf group list"
alias fglh = "dnf group list --hidden"
```
you can see more/whole into [fish_conf](https://github.com/alfinbudiyanto/fish_conf)

## Install RPM Fusion
```
sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
```
and then check dnf repo list first before enabling openh264
```
dnf repolist --enabled | grep fedora-cisco-openh264
```
if it show like `fedora-cisco-openh264 Fedora 44 openh264 (From Cisco) - x86_64` you are done, if not yet enabled, run this command
```
sudo dnf config-manager setopt fedora-cisco-openh264.enabled=1
```
For Fedora 41 and later!
