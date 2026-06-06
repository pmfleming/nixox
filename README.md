# NixOS Config

This repository tracks the live NixOS flake configuration in `/etc/nixos`.

## Apply Changes

Apply the ThinkPad configuration:

```sh
sudo nixos-rebuild switch --flake /etc/nixos#thinkpad
```

## Validate Changes

Check the flake before applying it:

```sh
nix flake check /etc/nixos --no-build
```

## Notes

- `hardware-configuration.nix` is machine-specific.
- Review `git diff` before committing or applying changes.
