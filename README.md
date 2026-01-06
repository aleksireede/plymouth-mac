# plymouth-mac
A macOS-like boot screen theme for Plymouth
## Installation

1. Clone this repo and then `cd` to it.

        $ git clone https://github.com/aleksireede/plymouth-mac.git && cd plymouth-mac
        
2. Copy **mac** folder to `/usr/share/plymouth/themes` directory and `cd` to there.

        $ sudo cp -r plymouth-mac /usr/share/plymouth/themes && cd /usr/share/plymouth/themes

3. Run the command below.
        
        $ sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/plymouth-mac/plymouth-mac.plymouth 100

4. arch linux version.

        $ sudo plymouth-set-default-theme

        
5. And then run:
        
        $ sudo update-alternatives --config default.plymouth
        
   to choose and set the default theme.

6. Finally, run:
        
        $ sudo update-initramfs -u
