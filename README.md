# AppArmor Profile for Anonymity Linux Distributions #

Displaces /etc/apparmor.d/abstractions/base with a version, that includes
additions required for Anonymity Linux Distributions.

Does not depend on AppArmor, so this package can be installed by default on
any anonymity distribution by default, without requiring to also have AppArmor
installed. Just for the case, AppArmor gets installed later by the user.
## How to install `apparmor-profile-dist` using apt-get ##

1\. Download the APT Signing Key.

```
wget https://www.whonix.org/derivative.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add the APT Signing Key..

```
sudo cp ~/derivative.asc /usr/share/keyrings/derivative.asc
```

3\. Add the derivative repository.

```
echo "deb [signed-by=/usr/share/keyrings/derivative.asc] https://deb.whonix.org bullseye main contrib non-free" | sudo tee /etc/apt/sources.list.d/derivative.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `apparmor-profile-dist`.

```
sudo apt-get install apparmor-profile-dist
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions. (Replace `generic-package` with the actual name of this package `apparmor-profile-dist`.)

* **A)** [easy](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package/easy), _OR_
* **B)** [including verifying software signatures](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`apparmor-profile-dist` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
