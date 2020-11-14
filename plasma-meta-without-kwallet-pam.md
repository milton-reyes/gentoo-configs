## Plasma 5 without kwallet-pam
#### When installing kde desktop environment in Gentoo it is recommended to install the kde-plasma/plasma-meta package for a full Plasma 5 desktop. This action will pull kwallet-pam which may be undesirable. Instead of installing the meta package you can install these individual packages for a functional kde plasma desktop environment without kwallet-pam
#### These are dependencies found specifically in kde-plasma/plasma-meta-5.19.5 ebuild meta package for installing kde plasma desktop environment
kde-plasma/breeze kde-plasma/drkonqi kde-plasma/kactivitymanagerd kde-plasma/kde-cli-tools kde-plasma/kdecoration kde-plasma/kdeplasma-addons kde-plasma/kgamma kde-plasma/khotkeys kde-plasma/kinfocenter kde-plasma/kmenuedit kde-plasma/kscreen kde-plasma/kscreenlocker kde-plasma/ksshaskpass kde-plasma/ksysguard kde-plasma/kwayland-integration kde-plasma/kwayland-server kde-plasma/kwin kde-plasma/kwrited kde-plasma/libkscreen kde-plasma/libksysguard kde-plasma/milou kde-plasma/oxygen kde-plasma/plasma-desktop kde-plasma/plasma-integration kde-plasma/plasma-workspace kde-plasma/polkit-kde-agent kde-plasma/powerdevil kde-plasma/systemsettings kde-plasma/user-manager kde-plasma/bluedevil kde-plasma/kde-gtk-config x11-misc/appmenu-gtk-module kde-apps/khelpcenter kde-plasma/plasma-pa kde-plasma/plasma-workspace-wallpapers


You could also install the meta package without flags

`echo "kde-plasma/plasma-meta -sddm -kwallet -browser-integration -display-manager" >> /etc/portage/package.use/plasmaMeta`

or

`USE="-sddm -kwallet -browser-integration -display-manager" emerge -av kde-plasma/plasma-meta`


