# blockauth-sdk
Block-Auth Auth SDK is a SASS service blockchain based authentication service. It provides a simple and secure way to authenticate users in your application.

DEVELOPMENT process is private yet, but will open source eventually

You can learn how to use here: [https://docs.block-auth.io/quickstart](https://docs.block-auth.io/quickstart/)


# JS client

```
# Install the Protocol JavaScript SDK
npm install blockauth-sdk --save
```

## Example of usage

```
import { BlockAuthProvider } from 'blockauth-sdk'

const provider = new BlockAuthProvider({
  apiKey: 'API_KEY',
  apiSecret: 'API_SECRET',
})
await provider.connect()
if (!provider.isConnected()) {
  throw new Error('Could not connect to Block-Auth')
}
await provider.signin()
```
