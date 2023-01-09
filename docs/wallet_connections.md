# Wallet Connections

Most Dapps use the [Lamden Vault](https://docs.lamden.io/docs) to send transactions on behald of the user.

To make your Dapp connect and send transctions to Arko you will provide a new `networkVersion` property in the wallet connection information.

### Legacy Lamden

```javascript
const detail = JSON.stringify({
    appName: 'My Killer dApp',
    version: '1.0.0',
    logo: 'images/logo.png',
    contractName: 'con_killer_app', 
    networkType: 'mainnet'
})

```

### Arko

```javascript
const detail = JSON.stringify({
    appName: 'My Killer dApp',
    version: '1.0.0',
    logo: 'images/logo.png',
    contractName: 'con_killer_app', 
    networkType: 'mainnet', 
    networkVersion: 2 // This tells the wallet to use Arko
})
```

This change should be make after Arko goes live. When people visit your Dapp they will be asked to create a new connection.

