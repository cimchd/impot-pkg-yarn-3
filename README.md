# import-pkg-yarn-3

Minimal reproduction repo for antfu/install-pkg and yarn v3 with preferOffline option.

Just run `yarn install` and then `node index.js`.

The following error should occur:

```sh
Unsupported option name ("--prefer-offline").

$ yarn add [--json] [-E,--exact] [-T,--tilde] [-C,--caret] [-D,--dev] [-P,--peer] [-O,--optional] [--prefer-dev] [-i,--interactive] [--cached] [--mode #0] ...
/home/chd/impot-pkg-yarn-3/node_modules/execa/lib/error.js:60
                error = new Error(message);
                        ^

Error: Command failed with exit code 1: yarn add --prefer-offline vite
```
