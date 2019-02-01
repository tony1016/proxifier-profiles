# Proxifier Profiles
A ruleset for Proxifier on OS X, founded by [Jamesits](https://github.com/Jamesits/proxifier-profiles).But the author want to REDUCE the power and I want to ENHANCE it.

## Features
Rules:

- Direct connection:
    - Other common proxy softwares (to prevent infinite loop)
    - Localhost
    - Link-local addresses and LANs (with IPv6 considered)
    - Common router management addresses (IPs and fake domains)
    - P2P download softwares
    - Chinese sites, via:
        - Common CDNs
        - Multimedia content providers
        - Domain whitelist
        - IP ranges
    - Other common district-restricted contents (Steam, etc.)
- Forced proxy:
    - Blocked services
        - Google, Dropbox, Gravatar, Wordpress, etc.
        - Categoried by service ,not apps
    - Unstable services
        - iTunes / App Store / iCloud
          (Plus, if your proxy have a data limit, you can filter out App Store downloads individually.)
        - Microsoft services
        - Services for programmers: Github, Homebrew, PyPI, Atom, Android SDK, etc.
        - Games: Minecraft, etc.
        - Common foreign CDNs
    - **All the NON-CHINESE web service**

These rules are split into individual items so you can simply enable or disable one using Proxifier's built-in mechanism, or redirect any of them to another proxy.

## Installation

By default Proxifier's profiles are stored under `~/Library/Application Support/Proxifier/Profiles`. Download `Profiles/Current.ppx` and put it in, then you should be able to load it via dropdown menu on the right of Proxifier's toolbar.

If you want to use Git like me, you can run the following commands in a shell:

```shell
git clone https://github.com/tony1016/proxifier-profiles.git ~/.proxifier-profiles
ln -s ~/.proxifier-profiles/Profiles/Current.ppx ~/Library/Application\ Support/Proxifier/Profiles/GiveMeABreak.ppx
```

## References
- See [Jamesits/chnroutes](https://github.com/Jamesits/chnroutes/tree/feature/proxifier) for Chinese IP ranges support.
