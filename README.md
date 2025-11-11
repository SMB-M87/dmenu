# dmenu
Suckless Dynamic Menu

git clone https://git.suckless.org/dmenu

cd ../dmenu

## Patches
curl -O https://tools.suckless.org/dmenu/patches/case-insensitive/dmenu-caseinsensitive-20200523-db6093f.diff

curl -O https://tools.suckless.org/dmenu/patches/grid/dmenu-grid-4.9.diff

curl -O https://tools.suckless.org/dmenu/patches/gridnav/dmenu-gridnav-5.2.diff

curl -O https://tools.suckless.org/dmenu/patches/mouse-support/dmenu-mousesupport-5.3.diff

curl -O https://tools.suckless.org/dmenu/patches/center/dmenu-center-20250407-b1e217b.diff

curl -O https://tools.suckless.org/dmenu/patches/alpha/dmenu-alpha-20250614-b1e217b.diff

## Initial Build
patch -p1 < patches/dmenu-caseinsensitive-20200523-db6093f.diff

patch -p1 < patches/dmenu-grid-4.9.diff

patch -p1 < patches/dmenu-gridnav-5.2.diff

patch -p1 < patches/dmenu-mousesupport-5.3.diff

patch -p1 < patches/dmenu-center-20250407-b1e217b.diff

patch -p1 < patches/dmenu-alpha-20250614-b1e217b.diff

make clean install
