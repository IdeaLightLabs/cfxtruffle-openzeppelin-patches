# cfxtruffle-openzeppelin-patches

The patches are created to make cfxtruffle work correctly with openzeppelin's upgradable contracts.

***Notice: The patches require the `truffle-cfx-patch` npm package to work. Please install `truffle-cfx-patch` and configure the project files FIRST.***

## Usage

1. Copy `*.patch` to the `/patches` folder of your project.

2. Add a script in `package.json`:
```json
"postinstall": "patch-package"
```

3. Install `patch-package`
```bash
yarn add -D patch-package
```

## Tested

The patches has been tested working fine with `cfxtruffle@1.0.2` / `@openzeppelin/truffle-upgrades@1.15.0`, both `deployProxy` and `upgradeProxy`.
