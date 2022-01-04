# Install Steps

1. `git clone https://github.com/atayebali/private-block-chain`

2. `npm install`

# Run
` node app.js` 


# Libraries 

Could not use the original libraries that were used project due to JS errors.  Had to use this set for `npm install` to run. 

```
   "bitcoinjs-lib": "^6.0.1",
    "bitcoinjs-message": "^2.2.0",
    "body-parser": "^1.18.3",
    "crypto-js": "^4.1.1",
    "express": "^4.16.4",
    "hex2ascii": "0.0.3",
    "morgan": "^1.9.1"
```

# Bitcoin Core 

Unable to sign transactions for ownership verification without making a change to the `bitcoin.conf` file.

