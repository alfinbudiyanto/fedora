# Fedora

```
╭─ wolfei@fedora ~
╰─❯ fgl --installed
Updating and loading repositories:
Repositories loaded.
ID                   Name        Installed
libreoffice          LibreOffice       yes
```
##### I prefer to install from flatpak
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
##### why only 4?,,
core is not count because it is fedora based

### For aliases was i made
alias fgl = "dnf group list"

alias fglh = "dnf group list --hidden"

you can see more/whole into [fish_conf](https://github.com/alfinbudiyanto/fish_conf)
