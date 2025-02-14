## Privacy Settings Menu GNOME Extension
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate?hosted_button_id=G2REEPPNZK9GN)
  - Add a privacy menu to the top bar for quick access to privacy settings in GNOME
  - Supports GNOME 3.38+, earlier versions are untested
  - Get the extension from [here](https://extensions.gnome.org/extension/4491/privacy-settings-menu/)
  - This project is licensed under GPL 3.0
  - Any donations are greatly appreciated :)

![Extension](docs/icon.png)

## Install the extension from releases:
  - Extract the zip to `~/.local/share/gnome-shell-extensions/PrivacyMenu@stuarthayhurst/`
  - Reload GNOME
  - Enable the extension

## Install the extension from source:
  - Make sure the install dependencies are installed
  - `make build`
  - `make install`
  - Reload GNOME
  - Enable the extension

## Build system usage:
  - ### Common targets: Regular build system targets to build, install and uninstall
    - `make build`: Creates extension zip
    - `make check`: Runs checks on built extension zip
    - `make install`: Installs the extension
    - `make uninstall`: Uninstalls the extension
  - ### Development targets: These targets are aimed at developers and translators
    - `make clean`: Deletes extension zip
    - `make translations`: Updates translations
    - `make prune`: Removes rubbish from any .svgs in `docs/`
    - `make compress`: Losslessly compresses any .pngs in `docs/`
    - `make release`: Updated translations, then creates and checks an extension zip

## Install dependencies:
  - gettext
  - gnome-extensions

## Build dependencies: (Only required if running `make release`)
  - `All install dependencies`
  - sed (`make translations`)
  - python3 (`make prune`)
  - optipng (`make compress`)

## Want to help?
  - Help with the project is always appreciated, refer to `docs/CONTRIBUTING.md` to get started
  - Documentation, code changes and translations are always welcome!
  - [Documentation](docs/CONTRIBUTING.md#documentation-changes), [code](docs/CONTRIBUTING.md#code-changes) and [translations](docs/CONTRIBUTING.md#translations) are always welcome!

## Bug reporting / debugging:
  - A live feed of GNOME's logs can be accessed with `journalctl /usr/bin/gnome-shell -f -o cat`
  - If the extension is crashing, an output from this is very helpful for fixing it

### Credits:
  - `scripts/update-po.sh` and `scripts/update-pot.sh` were derived from [Fly-Pie](https://github.com/Schneegans/Fly-Pie), originally licensed under the [MIT license](https://github.com/Schneegans/Fly-Pie/blob/develop/LICENSE)

### Screenshot:
![Extension](docs/screenshot.png)
