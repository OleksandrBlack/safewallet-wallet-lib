# safewallet-wallet-lib

### How to build Safewallet lib for client side

install browserify

browserify index.js --standalone safewallet > safewalletlib.js

### How to add btc compatible pow coin
- add coin network params in src/bitcoinjs-networks.js
- add electrum servers list and tx fee in src/electrum-servers.js

### How to add safe asset chain
- add electrum servers list and tx fee in src/electrum-servers.js
- add asset chain ticker and an explorer link in src/coin-helpers.js

### How build for old browsers (ES5)
install babel
npm install babel-preset-es2015

npm run build

example:
`var fromSats = require('safewallet-wallet-lib/build/utils').fromSats;`