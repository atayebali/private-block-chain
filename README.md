# Install Steps

1. `git clone https://github.com/atayebali/private-block-chain`

2. `npm install`

# Run
` node app.js` 


# Libraries 

Could not use the original libraries that were used project due to JS errors.  Had to use this set for `npm install` to run. 

```js
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

`addresstype = legacy`

Without added the setting above, bitcoin core will not sign transactions.


# Test Results

### Get block by height

Genesis block is fetched via API

<img width="833" alt="Screen Shot 2022-01-04 at 1 29 37 PM" src="https://user-images.githubusercontent.com/777379/148126367-94bfca04-5fc3-4e5c-a1d9-4040997e8d82.png">

### Post wallet address for validation

Request sends back a timestamped message that will be used to sign the tx on the blockchain.

<img width="930" alt="Screen Shot 2022-01-04 at 1 31 27 PM" src="https://user-images.githubusercontent.com/777379/148126530-5235a67d-aed5-49e1-8faa-f42b65f6fa43.png">

### Sign message with wallet 

Text returned from the API signed using bitcoin core ( see modification above needed to achieve this ).

<img width="758" alt="Screen Shot 2022-01-04 at 1 33 07 PM" src="https://user-images.githubusercontent.com/777379/148126726-e8bb496e-512b-4a8b-a0d1-63808e21d718.png">

## Post star object to the API for insertion into the blockchain

Payload includes wallet address and star object for adding to the private blockcchain

<img width="986" alt="Screen Shot 2022-01-04 at 1 34 42 PM" src="https://user-images.githubusercontent.com/777379/148126881-65883ceb-d87a-4c0b-b762-957891941cb5.png">

