# Alacritty configuration

Includes configuration for [alacritty][alacritty] (primarily for MacOS).

## Prerequisites

- alacritty (MaxOS only)

On MacOS, install Alacritty per the [docs][alacritty-install], then install the
Alacritty terminfo:

```bash
curl -o ~/alacritty.info https://github.com/alacritty/alacritty/blob/master/extra/alacritty.info && \
sudo tic -xe alacritty,alacritty-direct ~/alacritty.info && \
rm ~/alacritty.info
```

Finally, setup a font:
```bash
cat <<EOF > ~/.config/alacritty/font.toml
[font]
size = 10.0

[font.normal]
family = "RobotoMono Nerd Font Mono"
EOF
```

[alacritty]: https://alacritty.org/
[alacritty-install]: https://github.com/alacritty/alacritty/blob/master/INSTALL.md#terminfo
