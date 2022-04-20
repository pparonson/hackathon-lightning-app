# hackathon-lightning-app
* [hackathon-lightning-app] (https://github.com/pparonson/hackathon-lightning-app)

## Requirements
* Node 8+
* An [LND node](https://github.com/lightningnetwork/lnd)

## Setup the Project
Copy the environment configuration file with
```
cp .env.example .env
```

Edit the following fields in your new .env file with information about your node. You can get some help finding this info using this tool: https://lightningjoule.com/tools/node-info
* `LND_GRPC_URL` - The location to connect to your node. If you're running with default settings locally, this should be `127.0.0.1:10009`.
* `LND_MACAROON` - Your `readonly.macaroon` file, base64 encoded. Run `base64 readonly.macaroon` in your macaroon directory to get this.
* `LND_TLS_CERT` - Your TLS certificate, also base 64 encoded. Run `base64 tls.cert` in your data directory to get this.

## Run the Project
Install dependencies and run the app with
```sh
npm install && npm run dev
# OR #
yarn && yarn dev
```


