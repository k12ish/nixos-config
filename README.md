# Nix configurations

This repository is my first foray into nix, documented for my own ease of replication. I may occasionally rewrite history of this repository and force push.

At a high level, this repository started with the method outlined in (Vimjoyer's Ultimate Nix Guide)[https://www.youtube.com/watch?v=a67Sv4Mbxmc].

Other sources:
- https://nixos-and-flakes.thiscute.world/nixos-with-flakes/other-useful-tips#managing-the-configuration-with-git

## Replication

On a live NixOS instance:

1. Install `git` and set `nix.settings.experimental-features = [ "nix-command" "flakes" ];`
2. Clone this repo
3. Run:

```
sudo nixos-rebuild switch --flake .#default
```
