# picom-allusive
See [What is This](https://github.com/allusive-dev/picom-allusive#what-is-this)

Want to chat or maybe help bug test? Contatct me here:

[![Matrix](https://img.shields.io/badge/MATRIX-012121.svg?style=for-the-badge&logo=Matrix&logoColor=white)](https://matrix.to/#/@allusive_:matrix.org)
[![Discord](https://img.shields.io/badge/DISCORD-5865F2.svg?style=for-the-badge&logo=Discord&logoColor=white)](https://github.com/allusive-dev/allusive-dev#contact-me)
[![Email](https://img.shields.io/badge/EMAIL-160F33.svg?style=for-the-badge&logo=ProtonMail&logoColor=white)](mailto:jasper@allusive.dev)

Thanks very much for the support on this project recently, it really helps me stay motivated to keep working on it.
Can we get to 100 stars on GitHub next?

**If you are feelling really generous I now have GitHub sponsors setup so you can support my work more directly.
Even if you can only give a small amount it goes a long way!**

[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/allusive-dev)

### Announcements

Please check out the updated documentation.

Here is a full list of features that are now avaliable going ahead from `1.0`

- Includes all fixes and changes from `yshui/picom-v10.2`
- Includes pijulius animation code. (

    **As of `1.2.0` `animation-for-workspace-in`, `animation-for-workspace-out`, `animation-for-transient-window` have been removed because their corrosponding functions caused the issue of the wrong animations playing in all other instances.**

    If anyone has an issue with this please let me know in a issue.
  
  )
- Includes corners-rule. Allowing you to set the corner-radius on a per window basis.
- Animation open and unmap exclusion lists! Don't want something animating? Now you can fix that.
- Blur rules. Background blurring is now done on a whitelist basis to reduce hardware consumption.
- (As of `1.2.3`) fixes rounded corner issues on AwesomeWM.

## What Is This?

This was originally a fork of pijulius and nothing more, but since `1.0` this project has become much more and I hope it will go even further with your help. 

This is currently the best actively maintained fork of picom adding proper animations, implementing all features from upstream `v10.2` and adding more features as requested by the community!

## Documentation/Wiki.

The Wiki is also avaliable and actively updated on [Donument](https://donument.com/d/Allusive/picom-allusive/-/documents/) an up and coming git versioned database allows for more than just code to be versioned.

The GitHub Wiki is still actively maintained just incase, so don't worry about relying 100% on a external site yet if you don't feel comfortable with that. Thought I highly encourage taking a good look at Donument.

Can't find what you need in the wiki or have an problem? Open an Issue.

## Installation

### Building Manually
```
$ meson setup --buildtype=release . build
$ ninja -C build
$ ninja -C build install
```

### Arch Linux or other Arch based distros

```
$ paru -S picom-allusive
```
or
```
$ yay -S picom-allusive
```

### NixOS

picom-allusive is avaliable on unstable(23.11)

Keep in mind it can take up to a week after picom is updated before it will be avaliable on NixOS.

Simply do one of the following
``` nix
environment.systemPackages = [ pkgs.picom-allusive ];
```
or for home-manager
``` nix
home.packages = [ pkgs.picom-allusive ];
```

The package will not be avaliable on NixOS 23.05 You will have to wait until the next stable update if you are on the stable branch.

**If you still want to use picom and you are on 23.05 you can use the custom package (updated in the releases page) in either `environment.systemPackages` or `home.packages` for home-manager users. Keep in mind this is considerably unstable so expect possible issues.**

Thank you for your patience.
