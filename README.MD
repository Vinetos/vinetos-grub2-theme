# Vinetos Grub2 Theme

This theme is inspired by [ilham25/dotfiles-openbox](https://github.com/ilham25/dotfiles-openbox/) and based on [sandesh236/sleek--themes](https://github.com/sandesh236/sleek--themes).

# Screenshots :

> TODO

# Installation :

Install it as any other theme or on Nixos :
`/etc/nixos/configuration.nix` :

```nix
let
  vinetos-grub2-theme = builtins.fetchTarball {
    url = "https://github.com/Vinetos/vinetos-grub2-theme/releases/download/v0.0.1/vinetos-grub2-theme.tar.gz";
  };
in
{
  boot.loader = {
    grub = {
      theme = vinetos-grub2-theme;
      gfxmodeEfi = "1920x1080"; # You may need to force this setting
    };
  };
}
```
