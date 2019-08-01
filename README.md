# AppArmor Profile for Anonymity Linux Distributions #

Displaces /etc/apparmor.d/abstractions/base with a version, that includes
additions required for Anonymity Linux Distributions.

Does not depend on AppArmor, so this package can be installed by default on
any anonymity distribution by default, without requiring to also have AppArmor
installed. Just for the case, AppArmor gets installed later by the user.
## How to install `apparmor-profile-anondist` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `apparmor-profile-anondist`.

```
sudo apt-get install apparmor-profile-anondist
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `apparmor-profile-anondist` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`apparmor-profile-anondist` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
