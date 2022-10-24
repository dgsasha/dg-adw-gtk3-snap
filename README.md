<h1 align="center">
  <img src="images/icon.png" alt="dg-adw-gtk3-theme" width="156">
  <br />
  dg-adw-gtk3-theme
</h1>

<p align="center"><b>
  This is the snap for <a href="https://github.com/dgmarie/dg-adw-gtk3">dg-adw-gtk3</a></b>, <i>a Yaru inspired GTK3 theme</i>. 
</p>

<div align="center">

![dg-adw-gtk3-light](images/light.png?raw=true "dg-adw-gtk3-light")
![dg-adw-gtk3-dark](images/dark.png?raw=true "dg-adw-gtk3-dark")

</div>

## Install
```
sudo snap install dg-adw-gtk3-theme
```

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-white.svg)](https://snapcraft.io/dg-adw-gtk3-theme)

[Don't have snapd installed?](https://snapcraft.io/docs/core/install)

## Enabling GTK3 Theme
```
for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i dg-adw-gtk3-theme:gtk-3-themes; done
```

## Enabling Icon Theme
```
for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i dg-adw-gtk3-theme:icon-themes; done
```

## Enabling Sound Theme
```
for i in $(snap connections | grep gtk-common-themes:sound-themes | awk '{print $2}'); do sudo snap connect $i dg-adw-gtk3-theme:sound-themes; done
```