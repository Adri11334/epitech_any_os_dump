# Installation Epitech pour OS basés Debian (*buntu, Mint..), Archlinux, Fedora, Opensuse, Gentoo

# Contenu
- script d'installation **CSFML/SFML**
- script d'installation **criterion**
- script d'installation de **configuration minimale Epitech** (pour OS basés Debian (*buntu, Mint..), Archlinux, Fedora, Opensuse, Gentoo)

# Description

Ces scripts ont pour but de vous permettre de travailler sur vos projets EPITECH, depuis Manjaro (ou un autre OS que le dump du bocal).

Those installation script might work on any distribution based on :
- opensuse
- archlinux
- fedora
- debian
- gentoo

## Utilisation :

Placer l'iso dans une clé USB bootable, puis relancez votre pc dessus pour procéder à l'installation.

**Une fois sur votre nouvelle machine :**

```shell
$  sudo git clone git@github.com:Adri11334/epitech_any_os_dump.git /temp/dump

$  cd /temp/dump/EPITECH_STUFF/

$  sudo ./install <prenom.nom@epitech.eu>

$  sudo ./build_csfml

$  sudo ./install_criterion
```
Argument :
`<prenom.nom@epitech.eu>` : Votre login Epitech
<br>

#### Bonus:

* 1 - Installer pip
    * opensuse:
        ```shell
        sudo zypper install python3-pip
        ```
    * archlinux:
        ```shell
        sudo pacman -S python-pip
        ```
    * fedora:
        ```shell
        sudo dnf install python3-pip
        ```
    * debian:
        ```shell
        sudo apt install python-pip
        ```
    * gentoo:
        ```shell
        $  sudo emerge --ask dev-python/pip
        ```

* 2 - Installer les packages
    ```shell
    $  pip install gcovr

    $  pip install black

    $  pip install mypy
    ```



## Ce que font les scripts :

#### ./install
* mise à jour de votre système
* installation des paquets suivant :
    - blih
    - emacs (et la configuration epitech)
    - build-essentials (libc etc. pour compilation)
    - libncurses
    - curl
    - git
    - zsh
    - oh-my-zsh
    - terminator
    - valgrind
    - ocaml
    - tree
    - filezilla
    - man google (bonus)
* paquet en option :
    - makefile-gen
* génère et uploade votre **clé ssh sur le serveur epitech**
* change votre **shell de base en zsh**
* les **headers Epitech** contiennent le login même si le username sur la session est différent

#### ./build_csfml
* installation de **SFML 2.5.1**
* installation de **CSFML 2.5**

#### ./install_criterion
* installation de la lib criterion pour les **tests unitaires**

#### bonus
* installation de pip
* installation de gcovr
* installation de black
* installation de mypy

<br>
<br>

Pour toute suggestion, n'hesitez pas à ouvrir une **issue** (dans github)

<br>

> Le script 'install' a été écrit par **montag_p**, pour toute suggestion sur celui-ci, envoyer un mail à **paul[at]montague[dot]fr**
