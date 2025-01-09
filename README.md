### prerequisites

```bash
# smth may not be needed, needed to be clarified and extended
sudo pacman -S gst-plugins-good gst-plugins-bad gst-plugin-pipewire
yay -S gstreamer0.10-ffmpeg
```

### clone (and make changes)

```bash
git clone https://github.com/PodYapolskiy/sddm-fallout-theme.git && cd sddm-fallout-theme 
```

### test

```bash
sddm-greeter --test-mode --theme /usr/share/sddm/themes/sddm-fallout-theme
```

### add to sddm themes

```bash
sudo cp -r ../sddm-fallout-theme /usr/share/sddm/themes/
```

### change sddm theme

> edit /usr/lib/sddm/sddm.conf.d/default.conf in the following way

```conf
...
[Theme]
Current=sddm-fallout-theme
...
```