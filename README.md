## Hydro Protocol

[![CircleCI](https://circleci.com/gh/HydroProtocol/protocol/tree/master.svg?style=svg)](https://circleci.com/gh/HydroProtocol/protocol/tree/master)
[![codecov](https://codecov.io/gh/HydroProtocol/protocol/branch/master/graph/badge.svg)](https://codecov.io/gh/HydroProtocol/protocol)


> Hydro Protocol is an open-source framework for building decentralized exchanges on Ethereum.

![](./images/hydro_small.jpg)

Hydro is designed for developers looking to build decentralized exchanges without having to deal with the complexity and expense of designing, deploying, and securing their own smart contracts.

## Features

Hydro v2 has a lot of new features compared with v1. It supports lending, borrowing, margin trading, spot trading features.

* All great trading features in v1 version.
* A standalone funding pool to support margin trading, lending, borrowing.
* Built-in Funding insurance.
* Contract-deposit mode. Supports both ERC20 and Ether.
* Even less gas usage

Hydro v1 contains a single exchange contract called `HybridExchange.sol` with the following attributes:

* No order collision
* No possibility of front-running
* Accurate market orders
* Ability to collect fees as a percentage of the traded assets
* Allows asymmetrical maker/taker fee structure, rebates, discounts
* Multiple settlement models:
  * Wallet to wallet mode
  * Contract-deposit mode (supports ETH)
* Highly optimized gas usage

## Installation

```bash
npm install
```
To build json ABI files:

```bash
npm run compile
```

## Tests

```bash
npm run coverage
```

## Contributing

1. Fork it (<https://github.com/hydroprotocol/protocol/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

## License

This project is licensed under the Apache-2.0 License - see the [LICENSE.txt](LICENSE.txt) file for details

########################################################################################RES
########################################################################################
Microsoft Windows [Version 10.0.19041.1110]
(c) Microsoft Corporation. All rights reserved.

C:\Users\skull>cd desktop

C:\Users\skull\Desktop>cd testbox

C:\Users\skull\Desktop\TESTBOX>git clone https://github.com/AllSafeCybercurity/protocol.git
Cloning into 'protocol'...
remote: Enumerating objects: 3879, done.
remote: Counting objects: 100% (71/71), done.
remote: Compressing objects: 100% (57/57), done.
remote: Total 3879 (delta 41), reused 30 (delta 14), pack-reused 3808
Receiving objects: 100% (3879/3879), 1.29 MiB | 1.29 MiB/s, done.
Resolving deltas: 100% (2897/2897), done.

C:\Users\skull\Desktop\TESTBOX>cd protocol

C:\Users\skull\Desktop\TESTBOX\protocol>npm install
npm WARN old lockfile
npm WARN old lockfile The package-lock.json file was created with an old version of npm,
npm WARN old lockfile so supplemental metadata must be fetched from the registry.
npm WARN old lockfile
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile
npm WARN old lockfile Error: git dep preparation failed
npm WARN old lockfile     at ChildProcess.<anonymous> (C:\Program Files\nodejs\node_modules\npm\node_modules\@npmcli\promise-spawn\index.js:64:27)
npm WARN old lockfile     at ChildProcess.emit (node:events:394:28)
npm WARN old lockfile     at maybeClose (node:internal/child_process:1067:16)
npm WARN old lockfile     at Process.ChildProcess._handle.onexit (node:internal/child_process:301:5)
npm WARN old lockfile  Could not fetch metadata for websocket@git+ssh://git@github.com/frozeman/WebSocket-Node.git#6c72925e3f8aaaea8dc8450f97627e85263999f2 Error: git dep preparation failed
npm WARN old lockfile     at ChildProcess.<anonymous> (C:\Program Files\nodejs\node_modules\npm\node_modules\@npmcli\promise-spawn\index.js:64:27)
npm WARN old lockfile     at ChildProcess.emit (node:events:394:28)
npm WARN old lockfile     at maybeClose (node:internal/child_process:1067:16)
npm WARN old lockfile     at Process.ChildProcess._handle.onexit (node:internal/child_process:301:5) {
npm WARN old lockfile   cmd: 'C:\\Program Files\\nodejs\\node.exe',
npm WARN old lockfile   args: [
npm WARN old lockfile     'C:\\Program Files\\nodejs\\node_modules\\npm\\bin\\npm-cli.js',
npm WARN old lockfile     'install',
npm WARN old lockfile     '--force',
npm WARN old lockfile     '--cache=C:\\Users\\skull\\AppData\\Local\\npm-cache',
npm WARN old lockfile     '--prefer-offline=false',
npm WARN old lockfile     '--prefer-online=false',
npm WARN old lockfile     '--offline=false',
npm WARN old lockfile     '--no-progress',
npm WARN old lockfile     '--no-save',
npm WARN old lockfile     '--no-audit'
npm WARN old lockfile   ],
npm WARN old lockfile   code: 128,
npm WARN old lockfile   signal: null,
npm WARN old lockfile   stdout: '',
npm WARN old lockfile   stderr: 'npm WARN using --force Recommended protections disabled.\n' +
npm WARN old lockfile     'npm ERR! code 128\n' +
npm WARN old lockfile     'npm ERR! command failed\n' +
npm WARN old lockfile     'npm ERR! command git --no-replace-objects clone --mirror -q ssh://git@github.com/gulpjs/gulp.git C:\\Users\\skull\\AppData\\Local\\npm-cache\\_cacache\\tmp\\git-clone-77ef8d0b/.git --config core.longpaths=true\n' +
npm WARN old lockfile     "npm ERR! fatal: destination path 'C:\\Users\\skull\\AppData\\Local\\npm-cache\\_cacache\\tmp\\git-clone-77ef8d0b/.git' already exists and is not an empty directory.\n" +
npm WARN old lockfile     '\n' +
npm WARN old lockfile     'npm ERR! A complete log of this run can be found in:\n' +
npm WARN old lockfile     'npm ERR!     C:\\Users\\skull\\AppData\\Local\\npm-cache\\_logs\\2021-07-20T18_40_13_252Z-debug.log\n'
npm WARN old lockfile }
npm WARN deprecated mkdirp-promise@5.0.1: This package is broken and no longer maintained. 'mkdirp' itself supports promises now, please switch to that.
npm WARN deprecated tar.gz@1.0.7: ⚠️  WARNING ⚠️ tar.gz module has been deprecated and your application is vulnerable. Please use tar module instead: https://npmjs.com/tar
npm WARN deprecated har-validator@5.1.3: this library is no longer supported
npm WARN deprecated fs-promise@2.0.3: Use mz or fs-extra^3.0 with Promise Support
npm WARN deprecated debug@4.1.1: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm WARN deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated ethereumjs-tx@1.3.7: New package name format for new versions: @ethereumjs/tx. Please update.
npm WARN deprecated istanbul@0.4.5: This module is no longer maintained, try this instead:
npm WARN deprecated   npm i nyc
npm WARN deprecated Visit https://istanbul.js.org/integrations for other alternatives.
npm WARN deprecated truffle-hdwallet-provider@1.0.12: WARNING: This package has been renamed to @truffle/hdwallet-provider.
npm ERR! code 128
npm ERR! git dep preparation failed
npm ERR! command C:\Program Files\nodejs\node.exe C:\Program Files\nodejs\node_modules\npm\bin\npm-cli.js install --force --cache=C:\Users\skull\AppData\Local\npm-cache --prefer-offline=false --prefer-online=false --offline=false --no-progress --no-save --no-audit
npm ERR! npm WARN using --force Recommended protections disabled.
npm ERR! npm ERR! code 128
npm ERR! npm ERR! command failed
npm ERR! npm ERR! command git --no-replace-objects clone --mirror -q ssh://git@github.com/gulpjs/gulp.git C:\Users\skull\AppData\Local\npm-cache\_cacache\tmp\git-clone-5b6027be/.git --config core.longpaths=true
npm ERR! npm ERR! fatal: destination path 'C:\Users\skull\AppData\Local\npm-cache\_cacache\tmp\git-clone-5b6027be/.git' already exists and is not an empty directory.
npm ERR!
npm ERR! npm ERR! A complete log of this run can be found in:
npm ERR! npm ERR!     C:\Users\skull\AppData\Local\npm-cache\_logs\2021-07-20T18_42_55_670Z-debug.log

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\skull\AppData\Local\npm-cache\_logs\2021-07-20T18_43_33_163Z-debug.log

C:\Users\skull\Desktop\TESTBOX\protocol>npm audit fix
npm WARN old lockfile
npm WARN old lockfile The package-lock.json file was created with an old version of npm,
npm WARN old lockfile so supplemental metadata must be fetched from the registry.
npm WARN old lockfile
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile
npm WARN old lockfile Error: git dep preparation failed
npm WARN old lockfile     at ChildProcess.<anonymous> (C:\Program Files\nodejs\node_modules\npm\node_modules\@npmcli\promise-spawn\index.js:64:27)
npm WARN old lockfile     at ChildProcess.emit (node:events:394:28)
npm WARN old lockfile     at maybeClose (node:internal/child_process:1067:16)
npm WARN old lockfile     at Process.ChildProcess._handle.onexit (node:internal/child_process:301:5)
npm WARN old lockfile  Could not fetch metadata for websocket@git+ssh://git@github.com/frozeman/WebSocket-Node.git#6c72925e3f8aaaea8dc8450f97627e85263999f2 Error: git dep preparation failed
npm WARN old lockfile     at ChildProcess.<anonymous> (C:\Program Files\nodejs\node_modules\npm\node_modules\@npmcli\promise-spawn\index.js:64:27)
npm WARN old lockfile     at ChildProcess.emit (node:events:394:28)
npm WARN old lockfile     at maybeClose (node:internal/child_process:1067:16)
npm WARN old lockfile     at Process.ChildProcess._handle.onexit (node:internal/child_process:301:5) {
npm WARN old lockfile   cmd: 'C:\\Program Files\\nodejs\\node.exe',
npm WARN old lockfile   args: [
npm WARN old lockfile     'C:\\Program Files\\nodejs\\node_modules\\npm\\bin\\npm-cli.js',
npm WARN old lockfile     'install',
npm WARN old lockfile     '--force',
npm WARN old lockfile     '--cache=C:\\Users\\skull\\AppData\\Local\\npm-cache',
npm WARN old lockfile     '--prefer-offline=false',
npm WARN old lockfile     '--prefer-online=false',
npm WARN old lockfile     '--offline=false',
npm WARN old lockfile     '--no-progress',
npm WARN old lockfile     '--no-save',
npm WARN old lockfile     '--no-audit'
npm WARN old lockfile   ],
npm WARN old lockfile   code: 128,
npm WARN old lockfile   signal: null,
npm WARN old lockfile   stdout: '',
npm WARN old lockfile   stderr: 'npm WARN using --force Recommended protections disabled.\n' +
npm WARN old lockfile     'npm ERR! code 128\n' +
npm WARN old lockfile     'npm ERR! command failed\n' +
npm WARN old lockfile     'npm ERR! command git --no-replace-objects clone --mirror -q ssh://git@github.com/gulpjs/gulp.git C:\\Users\\skull\\AppData\\Local\\npm-cache\\_cacache\\tmp\\git-clone-aefe6ce5/.git --config core.longpaths=true\n' +
npm WARN old lockfile     "npm ERR! fatal: destination path 'C:\\Users\\skull\\AppData\\Local\\npm-cache\\_cacache\\tmp\\git-clone-aefe6ce5/.git' already exists and is not an empty directory.\n" +
npm WARN old lockfile     '\n' +
npm WARN old lockfile     'npm ERR! A complete log of this run can be found in:\n' +
npm WARN old lockfile     'npm ERR!     C:\\Users\\skull\\AppData\\Local\\npm-cache\\_logs\\2021-07-20T18_46_38_790Z-debug.log\n'
npm WARN old lockfile }
npm WARN audit fix mem@1.1.0 node_modules/@davidqhr/ganache-cli/node_modules/mem
npm WARN audit fix mem@1.1.0 is a bundled dependency of
npm WARN audit fix mem@1.1.0 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix mem@1.1.0 It cannot be fixed automatically.
npm WARN audit fix mem@1.1.0 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix yargs-parser@13.1.1 node_modules/@davidqhr/ethereumjs-testrpc-sc/node_modules/yargs-parser
npm WARN audit fix yargs-parser@13.1.1 is a bundled dependency of
npm WARN audit fix yargs-parser@13.1.1 @davidqhr/ethereumjs-testrpc-sc@6.4.2 at node_modules/@davidqhr/ethereumjs-testrpc-sc
npm WARN audit fix yargs-parser@13.1.1 It cannot be fixed automatically.
npm WARN audit fix yargs-parser@13.1.1 Check for updates to the @davidqhr/ethereumjs-testrpc-sc package.
npm WARN audit fix yargs-parser@9.0.2 node_modules/@davidqhr/ganache-cli/node_modules/yargs-parser
npm WARN audit fix yargs-parser@9.0.2 is a bundled dependency of
npm WARN audit fix yargs-parser@9.0.2 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix yargs-parser@9.0.2 It cannot be fixed automatically.
npm WARN audit fix yargs-parser@9.0.2 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix y18n@4.0.0 node_modules/@davidqhr/ethereumjs-testrpc-sc/node_modules/y18n
npm WARN audit fix y18n@4.0.0 is a bundled dependency of
npm WARN audit fix y18n@4.0.0 @davidqhr/ethereumjs-testrpc-sc@6.4.2 at node_modules/@davidqhr/ethereumjs-testrpc-sc
npm WARN audit fix y18n@4.0.0 It cannot be fixed automatically.
npm WARN audit fix y18n@4.0.0 Check for updates to the @davidqhr/ethereumjs-testrpc-sc package.
npm WARN audit fix y18n@3.2.1 node_modules/@davidqhr/ganache-cli/node_modules/y18n
npm WARN audit fix y18n@3.2.1 is a bundled dependency of
npm WARN audit fix y18n@3.2.1 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix y18n@3.2.1 It cannot be fixed automatically.
npm WARN audit fix y18n@3.2.1 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix os-locale@2.1.0 node_modules/@davidqhr/ganache-cli/node_modules/os-locale
npm WARN audit fix os-locale@2.1.0 is a bundled dependency of
npm WARN audit fix os-locale@2.1.0 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix os-locale@2.1.0 It cannot be fixed automatically.
npm WARN audit fix os-locale@2.1.0 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix yargs@11.1.0 node_modules/@davidqhr/ganache-cli/node_modules/yargs
npm WARN audit fix yargs@11.1.0 is a bundled dependency of
npm WARN audit fix yargs@11.1.0 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix yargs@11.1.0 It cannot be fixed automatically.
npm WARN audit fix yargs@11.1.0 Check for updates to the @davidqhr/ganache-cli package.
npm WARN deprecated mkdirp-promise@5.0.1: This package is broken and no longer maintained. 'mkdirp' itself supports promises now, please switch to that.
npm WARN deprecated har-validator@5.1.5: this library is no longer supported
npm WARN deprecated debug@4.1.1: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated istanbul@0.4.5: This module is no longer maintained, try this instead:
npm WARN deprecated   npm i nyc
npm WARN deprecated Visit https://istanbul.js.org/integrations for other alternatives.
npm WARN deprecated truffle-hdwallet-provider@1.0.17: WARNING: This package has been renamed to @truffle/hdwallet-provider.
npm ERR! code 1
npm ERR! path C:\Users\skull\Desktop\TESTBOX\protocol\node_modules\keccakjs\node_modules\sha3
npm ERR! command failed
npm ERR! command C:\WINDOWS\system32\cmd.exe /d /s /c node-gyp rebuild
npm ERR! gyp info it worked if it ends with ok
npm ERR! gyp info using node-gyp@7.1.2
npm ERR! gyp info using node@16.4.1 | win32 | x64
npm ERR! gyp info find Python using Python version 3.9.6 found at "C:\Users\skull\AppData\Local\Programs\Python\Python39\python.exe"
npm ERR! gyp ERR! find VS
npm ERR! gyp ERR! find VS msvs_version not set from command line or npm config
npm ERR! gyp ERR! find VS VCINSTALLDIR not set, not running in VS Command Prompt
npm ERR! gyp ERR! find VS could not use PowerShell to find Visual Studio 2017 or newer, try re-running with '--loglevel silly' for more details
npm ERR! gyp ERR! find VS looking for Visual Studio 2015
npm ERR! gyp ERR! find VS - not found
npm ERR! gyp ERR! find VS not looking for VS2013 as it is only supported up to Node.js 8
npm ERR! gyp ERR! find VS
npm ERR! gyp ERR! find VS **************************************************************
npm ERR! gyp ERR! find VS You need to install the latest version of Visual Studio
npm ERR! gyp ERR! find VS including the "Desktop development with C++" workload.
npm ERR! gyp ERR! find VS For more information consult the documentation at:
npm ERR! gyp ERR! find VS https://github.com/nodejs/node-gyp#on-windows
npm ERR! gyp ERR! find VS **************************************************************
npm ERR! gyp ERR! find VS
npm ERR! gyp ERR! configure error
npm ERR! gyp ERR! stack Error: Could not find any Visual Studio installation to use
npm ERR! gyp ERR! stack     at VisualStudioFinder.fail (C:\Program Files\nodejs\node_modules\npm\node_modules\node-gyp\lib\find-visualstudio.js:121:47)
npm ERR! gyp ERR! stack     at C:\Program Files\nodejs\node_modules\npm\node_modules\node-gyp\lib\find-visualstudio.js:74:16
npm ERR! gyp ERR! stack     at VisualStudioFinder.findVisualStudio2013 (C:\Program Files\nodejs\node_modules\npm\node_modules\node-gyp\lib\find-visualstudio.js:351:14)
npm ERR! gyp ERR! stack     at C:\Program Files\nodejs\node_modules\npm\node_modules\node-gyp\lib\find-visualstudio.js:70:14
npm ERR! gyp ERR! stack     at C:\Program Files\nodejs\node_modules\npm\node_modules\node-gyp\lib\find-visualstudio.js:372:16
npm ERR! gyp ERR! stack     at C:\Program Files\nodejs\node_modules\npm\node_modules\node-gyp\lib\util.js:54:7
npm ERR! gyp ERR! stack     at C:\Program Files\nodejs\node_modules\npm\node_modules\node-gyp\lib\util.js:33:16
npm ERR! gyp ERR! stack     at ChildProcess.exithandler (node:child_process:404:5)
npm ERR! gyp ERR! stack     at ChildProcess.emit (node:events:394:28)
npm ERR! gyp ERR! stack     at maybeClose (node:internal/child_process:1067:16)
npm ERR! gyp ERR! System Windows_NT 10.0.19041
npm ERR! gyp ERR! command "C:\\Program Files\\nodejs\\node.exe" "C:\\Program Files\\nodejs\\node_modules\\npm\\node_modules\\node-gyp\\bin\\node-gyp.js" "rebuild"
npm ERR! gyp ERR! cwd C:\Users\skull\Desktop\TESTBOX\protocol\node_modules\keccakjs\node_modules\sha3
npm ERR! gyp ERR! node -v v16.4.1
npm ERR! gyp ERR! node-gyp -v v7.1.2
npm ERR! gyp ERR! not ok

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\skull\AppData\Local\npm-cache\_logs\2021-07-20T18_50_19_899Z-debug.log

C:\Users\skull\Desktop\TESTBOX\protocol>npm audit fix --force
npm WARN using --force Recommended protections disabled.
npm WARN old lockfile
npm WARN old lockfile The package-lock.json file was created with an old version of npm,
npm WARN old lockfile so supplemental metadata must be fetched from the registry.
npm WARN old lockfile
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile
npm WARN old lockfile Error: git dep preparation failed
npm WARN old lockfile     at ChildProcess.<anonymous> (C:\Program Files\nodejs\node_modules\npm\node_modules\@npmcli\promise-spawn\index.js:64:27)
npm WARN old lockfile     at ChildProcess.emit (node:events:394:28)
npm WARN old lockfile     at maybeClose (node:internal/child_process:1067:16)
npm WARN old lockfile     at Process.ChildProcess._handle.onexit (node:internal/child_process:301:5)
npm WARN old lockfile  Could not fetch metadata for websocket@git+ssh://git@github.com/frozeman/WebSocket-Node.git#6c72925e3f8aaaea8dc8450f97627e85263999f2 Error: git dep preparation failed
npm WARN old lockfile     at ChildProcess.<anonymous> (C:\Program Files\nodejs\node_modules\npm\node_modules\@npmcli\promise-spawn\index.js:64:27)
npm WARN old lockfile     at ChildProcess.emit (node:events:394:28)
npm WARN old lockfile     at maybeClose (node:internal/child_process:1067:16)
npm WARN old lockfile     at Process.ChildProcess._handle.onexit (node:internal/child_process:301:5) {
npm WARN old lockfile   cmd: 'C:\\Program Files\\nodejs\\node.exe',
npm WARN old lockfile   args: [
npm WARN old lockfile     'C:\\Program Files\\nodejs\\node_modules\\npm\\bin\\npm-cli.js',
npm WARN old lockfile     'install',
npm WARN old lockfile     '--force',
npm WARN old lockfile     '--cache=C:\\Users\\skull\\AppData\\Local\\npm-cache',
npm WARN old lockfile     '--prefer-offline=false',
npm WARN old lockfile     '--prefer-online=false',
npm WARN old lockfile     '--offline=false',
npm WARN old lockfile     '--no-progress',
npm WARN old lockfile     '--no-save',
npm WARN old lockfile     '--no-audit'
npm WARN old lockfile   ],
npm WARN old lockfile   code: 128,
npm WARN old lockfile   signal: null,
npm WARN old lockfile   stdout: '',
npm WARN old lockfile   stderr: 'npm WARN using --force Recommended protections disabled.\n' +
npm WARN old lockfile     'npm ERR! code 128\n' +
npm WARN old lockfile     'npm ERR! command failed\n' +
npm WARN old lockfile     'npm ERR! command git --no-replace-objects clone --mirror -q ssh://git@github.com/gulpjs/gulp.git C:\\Users\\skull\\AppData\\Local\\npm-cache\\_cacache\\tmp\\git-clone-9705b7b2/.git --config core.longpaths=true\n' +
npm WARN old lockfile     "npm ERR! fatal: destination path 'C:\\Users\\skull\\AppData\\Local\\npm-cache\\_cacache\\tmp\\git-clone-9705b7b2/.git' already exists and is not an empty directory.\n" +
npm WARN old lockfile     '\n' +
npm WARN old lockfile     'npm ERR! A complete log of this run can be found in:\n' +
npm WARN old lockfile     'npm ERR!     C:\\Users\\skull\\AppData\\Local\\npm-cache\\_logs\\2021-07-20T18_57_26_519Z-debug.log\n'
npm WARN old lockfile }
npm WARN audit fix mem@1.1.0 node_modules/@davidqhr/ganache-cli/node_modules/mem
npm WARN audit fix mem@1.1.0 is a bundled dependency of
npm WARN audit fix mem@1.1.0 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix mem@1.1.0 It cannot be fixed automatically.
npm WARN audit fix mem@1.1.0 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix yargs-parser@13.1.1 node_modules/@davidqhr/ethereumjs-testrpc-sc/node_modules/yargs-parser
npm WARN audit fix yargs-parser@13.1.1 is a bundled dependency of
npm WARN audit fix yargs-parser@13.1.1 @davidqhr/ethereumjs-testrpc-sc@6.4.2 at node_modules/@davidqhr/ethereumjs-testrpc-sc
npm WARN audit fix yargs-parser@13.1.1 It cannot be fixed automatically.
npm WARN audit fix yargs-parser@13.1.1 Check for updates to the @davidqhr/ethereumjs-testrpc-sc package.
npm WARN audit fix yargs-parser@9.0.2 node_modules/@davidqhr/ganache-cli/node_modules/yargs-parser
npm WARN audit fix yargs-parser@9.0.2 is a bundled dependency of
npm WARN audit fix yargs-parser@9.0.2 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix yargs-parser@9.0.2 It cannot be fixed automatically.
npm WARN audit fix yargs-parser@9.0.2 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix y18n@4.0.0 node_modules/@davidqhr/ethereumjs-testrpc-sc/node_modules/y18n
npm WARN audit fix y18n@4.0.0 is a bundled dependency of
npm WARN audit fix y18n@4.0.0 @davidqhr/ethereumjs-testrpc-sc@6.4.2 at node_modules/@davidqhr/ethereumjs-testrpc-sc
npm WARN audit fix y18n@4.0.0 It cannot be fixed automatically.
npm WARN audit fix y18n@4.0.0 Check for updates to the @davidqhr/ethereumjs-testrpc-sc package.
npm WARN audit fix y18n@3.2.1 node_modules/@davidqhr/ganache-cli/node_modules/y18n
npm WARN audit fix y18n@3.2.1 is a bundled dependency of
npm WARN audit fix y18n@3.2.1 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix y18n@3.2.1 It cannot be fixed automatically.
npm WARN audit fix y18n@3.2.1 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix os-locale@2.1.0 node_modules/@davidqhr/ganache-cli/node_modules/os-locale
npm WARN audit fix os-locale@2.1.0 is a bundled dependency of
npm WARN audit fix os-locale@2.1.0 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix os-locale@2.1.0 It cannot be fixed automatically.
npm WARN audit fix os-locale@2.1.0 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit fix yargs@11.1.0 node_modules/@davidqhr/ganache-cli/node_modules/yargs
npm WARN audit fix yargs@11.1.0 is a bundled dependency of
npm WARN audit fix yargs@11.1.0 @davidqhr/ganache-cli@6.4.3 at node_modules/@davidqhr/ganache-cli
npm WARN audit fix yargs@11.1.0 It cannot be fixed automatically.
npm WARN audit fix yargs@11.1.0 Check for updates to the @davidqhr/ganache-cli package.
npm WARN audit No fix available for @davidqhr/ganache-cli@*
npm WARN audit Updating truffle to 5.4.1,which is outside your stated dependency range.
npm WARN audit Updating @davidqhr/solidity-coverage to undefined,which is a SemVer major change.
npm ERR! code ETARGET
npm ERR! notarget No matching version found for @davidqhr/solidity-coverage@undefined.
npm ERR! notarget In most cases you or one of your dependencies are requesting
npm ERR! notarget a package version that doesn't exist.

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\skull\AppData\Local\npm-cache\_logs\2021-07-20T18_57_27_138Z-debug.log

C:\Users\skull\Desktop\TESTBOX\protocol>npm run compile

> compile
> truffle compile


C:\Users\skull\Desktop\TESTBOX\protocol>npm run coverage

> coverage
> solidity-coverage

'solidity-coverage' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\skull\Desktop\TESTBOX\protocol>
