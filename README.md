# rn-patch-package

Collection of React Native patches using [patch-package](https://github.com/ds300/patch-package)

## How to use

Simply copy over patch files into `patches` folder and run `yarn patch-package` (or make `patch-package` a npm script and run it) to apply the patches. Check in the patches folder and the `package.json` file to source control.

You will also need to setup `postinstall` script in `package.json` to run `patch-package` after `yarn install` or `npm install` (for yarn v1).

```json
{
  "scripts": {
    "postinstall": "patch-package"
  }
}
```

Refer to [patch-package](https://github.com/ds300/patch-package) for more documentation.