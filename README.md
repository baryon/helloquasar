# Quasar App (helloworld)

A Quasar Framework app

## Install the dependencies
```bash
npm install
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)
```bash
quasar dev -m electron
```

When you change package.json then `npm install & quasar dev -m electron`

```
    "@quasar/app": "3.0.0-beta.15",
```
from .16 to the latest .22, 
```
    "@quasar/app": "3.0.0-beta.16",
```
you will got a compile error
```
% quasar dev -m electron

 Dev mode.......... electron
 Pkg quasar........ v2.0.0-beta.15
 Pkg @quasar/app... v3.0.0-beta.22
 Pkg webpack....... v5
 Debugging......... enabled

 Configured browser support (>= 87.68% of global marketshare):
 · Chrome for Android >= 90
 · Firefox for Android >= 87
 · Android >= 90
 · Chrome >= 80
 · Edge >= 87
 · Firefox >= 79
 · iOS >= 11.0-11.2
 · Opera >= 71
 · Safari >= 11.1

 App • Chaining "Renderer" Webpack config
 App • Chaining "Preload" Webpack config
 App • Chaining "Main" Webpack config
 App •  WAIT  • Compiling of "Renderer" in progress...
 App •  DONE  • "Renderer" compiled with errors • 7143ms



 App •  ERROR  •  Renderer  in ./node_modules/bsv/lib/crypto/hash.node.js

Module not found: Can't resolve imported dependency "crypto"
Did you forget to install it? You can run: npm install --save crypto

 App •  ERROR  •  Renderer  in ./node_modules/bsv/lib/encoding/bufferwriter.js

Module not found: Can't resolve imported dependency "assert"
Did you forget to install it? You can run: npm install --save assert

 App •  ERROR  •  Renderer  in ./node_modules/bsv/lib/hdprivatekey.js

Module not found: Can't resolve imported dependency "assert"
Did you forget to install it? You can run: npm install --save assert


 App •  COMPILATION FAILED  • Please check the log above for details.
 ```